# A Quick Guide to OmegaT

## Overview

tbd

## How to install OmegaT in your local machine

tbd

## How to translate using OmegaT

tbd

## How to use translation memory and why

tbd

## How to use glossary and why

tbd

## How to use machine translations

### How to install Microsoft Translator

You can install Microsoft Translator into OmegaT and fetch the machine translation automatically. Use the shortcuts of Ctrl/Command+M to fill the segment with the machine translation.

The following instructions are based on OmegaT 4.1.5. For the older and later versions, the configurations may be different. Please refer to the **User's Manual**.

### 1. Azure Account
You need an Azure Account to subscribe to the Microsoft Translator in Microsoft Azure Marketplace. OmegaT needs the subscription key to utilize Microsoft Translator.
1. Access the Translator Text page on  [Microsoft Azure Marketplace](https://azuremarketplace.microsoft.com/en-us/marketplace/apps/Microsoft.CognitiveServicesTextTranslation?tab=Overview ). If the link is invalid, please search the Microsoft Azure Marketplace for the right page.
2. Sign in with your account or create a new account following the registration steps.
* You may need a new account to access the free trial.
3. Subscribe to Microsoft Translator Text and pick the pricing tier of F0.
* F0 provides machine translation of up to 2,000,000 characters per month for free, which is enough for AI Team translation job (for now).
* You can choose other tiers suitable for your need, which may require additional payment and credit card registration. 

*The details may change after certain updates in the user's interfaces or pricing strategies. If you encounter any problems, please contact IT before any uncertain configurations. * 

### 2. API key
After the subscription, you can generate the keys to activate Microsoft Translator in your OmegaT, following these steps:
1. Click the **Translator Service** in your **Azure Dashboard**.
2. Click **Resource Management** > **Keys**.
3. **Key 1** and **Key 2** will be generated automatically. 
* It may take a few minutes for the newly (re)generated keys to take effect.

### 3. Activate the plug-in
OmegaT needs your subscription key to implement the Mircosoft Translator. The configuration may be slightly different if you use a different version.
1. Click **Options** > **Preferences** > **Machine Translation** in your OmegaT.
2. Check the **Automatically fetch translations** box.
3. Choose **Microsoft Translator** in the Providers and then click **Configure**.
4. Paste your subscription key from Microsoft Translator into the corresponding blank.
5. Check the **Neural machine translation** box if you want to fetch the machine translation of NMT.
* You can check the details about **Neural Machine Translation** (NMT) and **Statistical Machine Translation** (SMT) in the [Microsoft Translator Documentation](https://docs.microsoft.com/zh-cn/azure/cognitive-services/translator/translator-info-overview). In short, NMT exceeds SMT in the translation quality, especially for Chinese and some other languages.
7. Click **Confirm**.

Now, you have utilized Microsoft Translator in your OmegaT. You can open a project and test the machine translation. 

- If you encounter any issues concerning the machine translation service, please contact IT or Microsoft Azure.

### 4. Usage limit

The Quota of 2,000,000 characters per month is sufficient for most personal projects and small/micro businesses. 

You can check your usage and the quota on your Microsoft Azure Dashboard by the following steps:

1. Click the **Cognitive Services** > **Overview** on your **Dashboard**.
2. Check the **Quota Info** on the bottom of the page.
3. The **Free tier include quantity Total** display your usage limit; the **Free tier include quantity Remaining** displays the quota left. 

Or you can view your detailed usage by hours by following steps:

1. Click the **Cognitive Services** > **Metrics** on your **Dashboard**.
2. Click **Add metric** and select the corresponding **Resource**, **Metric Namespace**, **Metric** (Characters Translated), **Aggregation** (Sum).
3. You can configure alerts for this metric by clicking **More** > **Configure alerts**. 
   * You need to pay for the automatic alerts. 

## How to contact OmegaT

If you encounter any issues concerning OmegaT, please contact the developers by the following approaches:

1. [Yahoo Group](https://groups.yahoo.com/neo/groups/OmegaT/info) (recommended)

2. [SourceForge](https://sourceforge.net/projects/omegat/support)

You can also get support from other OmegaT users on [Proz.com](https://www.proz.com/forum/omegat_support/).
