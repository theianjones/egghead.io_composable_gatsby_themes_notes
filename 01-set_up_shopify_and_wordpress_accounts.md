# 01. Set up a Shopify Account

[Code Link](https://github.com/christopherbiscardi/advanced-gatsby-themes-workshop-code/tree/master)

[Video Link](https://egghead.io/lessons/gatsby-set-up-a-shopify-account#t=0)

## Summary

To run the example project, we'll need to set up a shopify partner account, which is what they call their developer accounts.

## Notes

[00:00](https://egghead.io/lessons/gatsby-set-up-a-shopify-account#t=0) Set up your Shopify account at [Shopify Partners program](https://www.shopify.com/partners). Shopify Partner is what Shopify calls their developers.

Create a development store, Chris calls his Corgi Supply Inc.

[00:50](https://egghead.io/lessons/gatsby-set-up-a-shopify-account#t=50) **Set up a Product in your store**, he uses corgi stickers.

[01:04](https://egghead.io/lessons/gatsby-set-up-a-shopify-account#t=64) Now we want to go to Apps (in the side bar) -> manage private apps -> **create new private app**.

[01:20](https://egghead.io/lessons/gatsby-set-up-a-shopify-account#t=80) By default, you have most of the access that you need, but we'll also need to enable the store for an API at the bottom. After enabling the store for an API, make sure that you have Read product tags also enabled in the Read products, variants, and collections option and save.

[01:34](https://egghead.io/lessons/gatsby-set-up-a-shopify-account#t=94)  We use the **Storefront access token in our app** but copy that for later.

[01:53](https://egghead.io/lessons/gatsby-set-up-a-shopify-account#t=113) The plugin we'll be using is [Gatsby Source Shopify](https://github.com/angeloashmore/gatsby-source-shopify) and the permissions can be found in How to Use section of the Read Me.

# 02. Set up a WordPress Account

[Video Link](https://egghead.io/lessons/gatsby-set-up-a-wordpress-account#t=00)

## Summary

Set up the wordpress.com account needed for the course.

## Notes

[0:00](https://egghead.io/lessons/gatsby-set-up-a-wordpress-account#t=00) [Go to WordPress.com](https://wordpress.com/start/user?ref=logged-out-homepage-lp), sign up and **choose a Blog**, choose the topic of Blogging, and Chris calls his blog Corgi Co Blog.

[00:44](https://egghead.io/lessons/gatsby-set-up-a-wordpress-account#t=44) **Now our site has been created. We'll skip updating the home page, skip the tagline, and confirm our email address.**

[1:13](https://egghead.io/lessons/gatsby-set-up-a-wordpress-account#t=73) [gatsby-source-wordpress](https://www.gatsbyjs.org/packages/gatsby-source-wordpress/).

There's an option for hosting wpcom app

```js
// https://www.gatsbyjs.org/packages/gatsby-source-wordpress/
auth: {
wpcom_app_clientSecret: process.env.WORDPRESS_CLIENT_SECRET
wpcom_app_clientId: "54793",
wpcom_user: "gatsbyjswpexample@gmail.com",
wpcom_pass: process.env.WORDPRESS_PASSWORD,
}
```

To do this, **we have to create an app at **[developer.WordPress.com/apps](https://developer.wordpress.com/apps).

[1:35](https://egghead.io/lessons/gatsby-set-up-a-wordpress-account#t=95) Click on Create a new application. Give your application a name with the Description of something. The website URL doesn't matter. I'm going to use my personal site. **Note that all of the fields are required even if we're not going to use them**. You will have to specify a valid redirect URL in the form of HTTPS and a valid JavaScript origin.

[2:02](https://egghead.io/lessons/gatsby-set-up-a-wordpress-account#t=122) Note that **we'll need the WORDPRESS_CLIENT_SECRET and the clientId**.
