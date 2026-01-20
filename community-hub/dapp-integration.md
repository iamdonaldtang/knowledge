# DAPP integration

Through DAPP integration, you can embed GTC’s functionality into your official website, enabling website visitors to participate in the task incentive system. This connects your website (product), social media, and community through the task incentive system, fostering a stronger sense of community identity.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcYGYLDsArLQx8rlGdeuFYIA42BB25G_CGj8yWjqCpHFy0bo6-my3Yu_dYIzx59rkSolIEwvPMh2o4XinIDKp97uj9HZrkkrBxxqonm03SbDOmjw-51tYlry5uxZVFmaWnBghQ5Pw?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXe4fY1APCpwtlmCoOyW3agvngHtNrmsnx8amys15ByhXJEqIiJx_OYjWtqhSO1daAg7rHjuXylgkTZILf5BXXcK8oV_mlWV2dyzrSv_ygyUZqRec7SxAe_viDcyeLI67-k_GHWJjw?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

## Introduction <a href="#introduction" id="introduction"></a>

This guide walks you through the process of setting up a subdomain to redirect to the TaskOn community page via your domain provider's DNS configuration.

### Step 1: DNS Configuration <a href="#step-1-dns-configuration" id="step-1-dns-configuration"></a>

#### **Prerequisites**

* Access credentials: ensure you have access credentials for your domain's DNS settings.
* Subdomain selection: decide on the subdomain you wish to configure (e.g., subdomain.example.com).

_Note: Only subdomains can be used to serve your community page. It’s not possible to use an apex domain. Here are some examples of what you could and could not choose — just replace `example.com` with your own domain:_

| Domain type      | Example                                             | Supported? |
| ---------------- | --------------------------------------------------- | ---------- |
| Apex domain      | [example.com](http://example.com)                   | ❌          |
| www subdomain    | [www.example.com](http://www.example.com)           | ❌          |
| Custom subdomain | [anything.example.com](http://anything.example.com) | ✅          |

By accessing your domain provider's control panel and navigating to the DNS settings section, you will be modifying DNS settings:

| Type  | Name          | Value/Target              |
| ----- | ------------- | ------------------------- |
| CNAME | YourSubdomain | taskonsaas-prod.pages.dev |

Below are links to guides from major domain name service providers on how to add CNAME records for your domain:

* **GoDaddy:** [How to Add a CNAME Record](https://www.godaddy.com/en/help/add-a-cname-record-19236)
* **Cloudflare:** [Setting up CNAME with Cloudflare](https://developers.cloudflare.com/dns/zone-setups/partial-setup/)
* **Namecheap:** [Creating a CNAME Record for Your Domain with Namecheap](https://www.namecheap.com/support/knowledgebase/article.aspx/9646/2237/how-to-create-a-cname-record-for-your-domain/)
* **Domain.com:** [DNS Management - How to Update CNAME Records on Domain.com](https://www.domain.com/help/article/dns-management-how-to-update-cname-aliases)

Please follow the respective guide according to your domain provider to configure your CNAME settings.

### Step 2: Verify Configuration <a href="#step-2-verify-configuration" id="step-2-verify-configuration"></a>

After saving your DNS changes, use one of the following methods to verify your configuration:

1. **Check with TaskOn:** This is the recommended method for ease and reliability.
2. **Check with Third-Party Tools:** Use tools like [DNS Checker](https://dnschecker.org/)[DNS Map](https://dnsmap.io/)
3. **Use the Terminal:** For a more hands-on approach, directly query your DNS records using terminal commands.

<pre class="language-sh"><code class="lang-sh"><strong>    dig CNAME yoursubdomain.example.com +short
</strong></code></pre>

#### Additional Notes <a href="#additional-notes" id="additional-notes"></a>

Remember, DNS changes may take 24-48 hours to fully propagate. Contact [TaskOn support](https://t.me/Clairewhitee)

#### FAQ of Subdomain setup <a href="#faq-of-subdomain-setup" id="faq-of-subdomain-setup"></a>

**Why is my domain not verified?**

When you update the DNS records as part of the custom domain verification process with TaskOn, the changes usually take some time to propagate globally. Typically, this process is much faster than the standard DNS propagation times and often completes within 3 to 5 minutes. However, it's important to note that in some cases, depending on your domain registrar and the specific DNS changes made, it could take longer. During this waiting period, your custom domain will appear as unverified in TaskOn until the propagation is fully complete and the system can verify the changes.

**Why can't I access my website even though my domain is verified?**

If you've recently updated DNS records and can't access your site—even though the TaskOn Dashboard indicates the domain is configured correctly—it's likely due to a cached DNS record on your device or network. Testing this on a different device or internet connection can help, such as using a smartphone with mobile data. DNS caches clear automatically after a period (1-24 hours), but you can also manually reset your device or network equipment.

**Why has my domain been verified by a third-party tool but not by TaskOn?**

If third-party tools show your domain as verified but TaskOn does not, it's best to contact [TaskOn support](https://t.me/Clairewhitee)

