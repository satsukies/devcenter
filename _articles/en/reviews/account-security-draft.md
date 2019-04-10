---
title: Account Security- draft
redirect_from: []
date: 2019-04-10 09:10:48 +0000
published: false

---
## Enabling Two-factor authentication

We provide an extra layer of security if you enable Two-factor authentication (TFA) on your Bitrise account.

1. Download and install [Google Authenticator](https://support.google.com/accounts/answer/1066447?hl=en) on your phone.
2. Log in to [bitrise.io](https://www.bitrise.io) and go to your `Profile`.
3. Click `Account settings`.
4. Scroll down and click `Security` on the left.
5. Click on `Enable` under `Two-factor authentication`.
6. Open your Google Authenticator and scan the QR-code that appears on your screen.
7. Enter the 6-digit code that was generated.
8. Once you have activated your TFA and saved your recovery codes, you will receive a confirmation email from `letsconnect@bitrise.io`.

{% include message_box.html type="note" title="TFA on connected accounts" content=" We recommend that you check your connected accounts (GitHub, Bitbucket, GitLab and Xamarin) and enable TFAs if you haven't already. "%}

## Disabling Two-factor authentication

Follow this procedure to disable two-factor authentication if you are already logged into Bitrise.

1. Log in to [bitrise.io](https://www.bitrise.io) and go to your `Profile`.
2. Click `Account settings`.
3. Scroll down and click `Security` on the left.
4. Click on `Disable` under `Two-factor authentication`.

   ![](/img/disable-tfa.png)
5. Provide your Bitrise login password in the pop-up window.

   ![](/img/provide-password-2fa.jpg)

Now two-factor authentication is disabled.

### What to do if you have lost your authenticator and recovery codes 

2FA protects your account from unwanted login attempts (for example, with a stolen password) by providing an extra security step at the end of the login flow. Therefore, in the case of a lost phone, if you request us to disable 2FA and provide your password, we will not remove the activated 2FA from your account. 

However, if there has been any third-party service (for example, GitLab, GitHub or Bitbucket) connected to your account before, you can try to log in through that. In the absence of a connected third-party account, we recommend you to create a new account on Bitrise.

In very special cases, Bitrise can remove 2FA from your account. Please note that Bitrise can only disable the activated 2FA on your account, if there is a public repo on your git account **already connected to Bitrise**. 

1. Contact our Support Team using the email address you provided when signing up to Bitrise.
2. Explain why you're requesting us to remove 2FA.

   Our Support Team will ask you to create a new public repo on your git account with the title: `bitrise_verification`
3. Send the link of the created repo to our Support Team.

Our Support Team will remove 2FA on your account. 

Please note that our Support Team can deny your request if they find removing 2FA from the account might pose a security risk.

## Generating personal access tokens manually

There are two types of personal access tokens in your `Security` tab of your profile:

* the `auto-generated` ones, which are generated by Bitrise automatically whenever communicating with the Bitrise API
* the `user-generated` ones which you can manually generate for yourself

Follow the steps to create a new token manually!

1. In your `Security` tab, click on `Generate new`.
2. Fill out the `Token description` field and select the appropriate expiration time (1 hour, 1 day, 1 month or never) for your token.
3. Click `Save & Continue`.
4. In the `Personal Access token` pop-up window, you can see your newly generated token. Save it somewhere safe now so that you can use it later.
5. Click `Done`.

In your `Security` page, now you can see all your tokens with their expiration date and with the option to `Edit` or `Remove` them.