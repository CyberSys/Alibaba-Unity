# Alibaba-Unity
> Currently, this plugin is only suported on versions of Unity 2022.x and above

# Installation

This plugin is provided as a custom Unity package that you can import into any existing project with the Unity version 2022.x and above.

Once you've downloaded the Unity package, you can drag the `AlibabaManager.prefab` into your scene (inside the `AlibabaCloud` folder). 

---

# Setup

Alibaba Cloud provides an alternative to ChatGPT for Unity developers. 


### Step 1: Login to your Alibaba Cloud account and create an application in your dashboard
To get started you will first need to fetch your Application ID, which can be found in the Alibaba Cloud Platform under `My Application` (or through [this direct link](https://bailian.console.alibabacloud.com/#/app-center)). Here, you can create a new Application and copy the ID value (you will need this ID for the next step).

![](/Images/Screenshot1.JPG)

### Step 2: Inside your Alibaba Cloud account, create an API key
To continue you will need to fetch your API key, which can be found in your account under `API-KEY` (or through [this direct link](https://bailian.console.alibabacloud.com/?apiKey=1)). Here, you can create a new API KEY (you will need this API KEY for the next step too).


### Step 3: Open the Unity Editor, configure the package, and start using Alibaba Cloud
Inside the package, you will find an `AlibabaManager.prefab` that you can drag into your Scene. This prefab contains a `AlibabaAPI.cs` script attach to it. Add your API Secret Key inside the `API Key` field, and your application ID inside the `App ID`. And, you can start using Alibaba Cloud.

![](/Images/Screenshot2.JPG)


# Functions

This plugin provides one main function called `SendPrompt(string promptText)`. This function contains an IEnumerator, `IEnumerator SendPromptRequestToDashScope()`, which sends a prompt to the Alibaba Cloud API and prints the response to the console by calling Debug.Log().

Unity connects with Alibaba API through https://dashscope-intl.aliyuncs.com/api/v1/apps/{0}/completion. 


# Usage
After hitting on play, your Scene grabs the prompt you set inside `Your prompt` variable, and sends it to the Alibaba Cloud API. 

You must purchase credits in your Alibaba Cloud account to use the API. Nevertheless, they might be cheaper than ChatGPT API. 

Alibaba Cloud might offer you a Free Trial during the first 30 days. 

![](/Images/Screenshot2.JPG)


> Note that Alibaba Cloud is a paid API, I recommend using [Gemini](https://github.com/UnityGameStudio/Gemini-Unity-Package) instead, which is free upon certain amount of requests.
