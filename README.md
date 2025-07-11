# Hey there 👋

# Next JS tailwind CSS Ecommerce Checkout Page 

This example uses the [Flags SDK](https://flags-sdk.dev) along with the [Flags Explorer](https://vercel.com/docs/workflow-collaboration/feature-flags/using-vercel-toolbar) and `@vercel/analytics`.

## Demo

[https://shirt-shop.labs.vercel.dev/](https://shirt-shop.labs.vercel.dev/)

## How it works

This demo uses two feature flags defined in code control the visibility of two banners on the page.
Both flags are configured to show/hide each banner 50% of the time.

Once you visit the page, you can see a variation of both/one/none of the banners.
Since this example is using a stable id to identify users, you will see the same variation all the time.

To test different variations, you can use the Dev Tools at the bottom to reset the stable id and reload the page.
This allows you to test different variations of the banners.

This templates also tracks analytics events in Vercel Analytics.

If you deployed your own instance of this example you can also use the [Flags Explorer](https://vercel.com/docs/workflow-collaboration/feature-flags/using-vercel-toolbar) to test different variations by creating overrides.

## Deploy this template

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fvercel%2Fflags%2Ftree%2Fmain%2Fexamples%2Fshirt-shop&env=FLAGS_SECRET&envDescription=The+FLAGS_SECRET+will+be+used+by+the+Flags+Explorer+to+securely+overwrite+feature+flags.+Must+be+32+random+bytes%2C+base64-encoded.+Use+the+generated+value+or+set+your+own.&envLink=https%3A%2F%2Fvercel.com%2Fdocs%2Fworkflow-collaboration%2Ffeature-flags%2Fsupporting-feature-flags%23flags_secret-environment-variable&project-name=shirt-shop-flags-sdk-example&repository-name=shirt-shop-flags-sdk-example)

### Step 1: Link the project

In order to use the Flags Explorer, you need to link the project on your local machine.

```bash
vercel link
```

Select the project from the list you just deployed.

### Step 2: Pull all environment variables

This allows the Flags SDK and the Flags Explorer to work correctly, by getting additional metadata.

```bash
vercel env pull
```

### Step 3: Install dependencies

```bash
npm install
```

### Step 4: Run the project

```bash
npm run dev
```
