# API Task

## Use Cases and Logic

TaskOn enables seamless integration of APIs with various applications and functions to verify whether participants are using your product or specific features, including but not limited to liquidity provision, borrowing, supplying, mining, and swapping.

To use an `API-Verified Task`, you must provide a Task Description and configure the API URL.

TaskOn’s API verification task feature integrates APIs from various applications and functions. When using API-verified tasks, first select whether it’s a _Performance-Based API Task_ or a _Completion-Based API Task_.

### **Completion-Based API Task**:&#x20;

Focuses on task completion status, verified through an API interface. Project teams can indicate which wallet addresses have completed the task. Behaviors such as app downloads or user registrations can be rewarded through API settings in this module.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfY1C5RdjicocTjzoRdCdEnVK1hd9TVjBCKbXrdW9evpQzJKuco6M9CMp5LpIAJDwrAfmOZfxpzOxVRJyYsfJ4TIOn26z8cUwQkukbK4xtKm3DZ_Zwh1oU3emd9AOt89TGzhRGqIQ?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

### **Performance-Based API Task:**&#x20;

Focuses on dynamic point rewards. Project teams can set periodic reward actions via the API interface to specify which user actions qualify for ongoing rewards. For example, if you want users to log into your official account daily or interact with your website, with different interactions yielding different rewards, you can configure this through the API module.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXfN774Rt60O-2qCyTcpvV3Y2hiPnB8clmIexxlUGOuzC01FlRSFB2fm-9Jh8Acw5baKY3WT1M17OJy3U20rfXBmRde-s95ulIRO0Diu2GN6boR0nvqvmkl03qcB0izyoCKK-7TTlA?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

## Steps

### Step 1:

Click “Set API URL,” then select [API Standards Specification](https://versed-catshark-f4d.notion.site/Instructions-on-How-to-Integrate-External-APIs-for-TaskOn-Task-Verification-1f854c607cd349948c8db6f108fc39f1) to access the information needed to integrate TaskOn’s task verification with an external API.

### **Set API URL**:

You can choose between social media accounts or wallet addresses.

For social media accounts, select from X, Discord ID, Telegram ID, or email, and provide a valid API URL for task verification.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXdoZ6z5k0-8177KqeC5TChrNaHYS2St8et621HDtheJgWj0HZ52pJxYEzxyLEgCY-Vgn9y5rcwWEW4VwhnAQNHcpAa1syT8ysySm7urnkm18Hd7ObhpVswlLuKNTNM8N49b9z2CbA?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

For wallet addresses, select the appropriate network.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXc0xL_gD6qTj3vn22oFxIlmYxLhZajhO5wMhUTffF9nEYYq4BBx4mTMUgo0HjD5QLENjvZSbx7wUWbWKoNrdt6SNceY5RAALK6ds2c5Zd0D2t2nBfXB7nZVbL7Ve2bXS_YjoHE7dw?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

### Step 2:&#x20;

Verification Configuration and Wallet Address Input

For Completion-Based API Tasks, you can upload lists of qualified and unqualified wallet addresses. For Performance-Based API Tasks, you can upload qualified wallet addresses. The system requires qualified wallet addresses to mark eligibility, automatically recording verified addresses. Rewards are distributed based on associated addresses, while data isolation is effectively maintained at the data layer, generating a participation data dashboard.

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXcq1SgherYfdTQxYp-TnVgacQQZiUcS4n6XjIidQtKNqVYKsi-f2w1tJSrWcvlG6N9unyzvTR8daS5FtYcg8J-1aO2gGRU0nJZyISIV5zWwwpbqHrzCfQZdMpFsB3Di3Z5NvXCq?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>

<figure><img src="https://lh7-rt.googleusercontent.com/docsz/AD_4nXezsCI1j4exIeAa8MlyA0PbuQziALeWaorJMcObe-Hck0Tkn3faZCaPsTMlbdwr9bsg2EdTsAHkNkXn2zA6WXypyIFpnYFshQtISq9xJeeNP0UVoO9mMGj8Z95XqoMluH2EaV7R?key=0Ugs8HwP_vZfQwQiqIZ9vA" alt=""><figcaption></figcaption></figure>
