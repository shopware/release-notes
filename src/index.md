---
items:
  - text: Overview
    link: "../../release-notes/src/index.md"
meta:
  orientation: descending
items:
  - text: References
    items:
      - text: GitHub releases
        link: "https://github.com/shopware/shopware/releases"
      - text: Forum news
        link: "https://forum.shopware.com/"
      - text: Changelog
        link: "https://www.shopware.com/en/changelog/"
      - text: Security audit report
        link: "https://github.com/shopware/shopware/security/advisories?state=published"
---

# Shopware Release Policy

## Release management at Shopware

Releasing new versions of Shopware is essential to stay competitive in the market and offer merchants benefits through the introduction of new features, adjustments to existing ones, or enhancements to the underlying architecture of Shopware.

Knowing that each update requires effort from the community, we are careful to minimize its impact. The following overview of our release strategy provides insight into what you can expect.

## Shopware SaaS, PaaS and Self-Hosted

Shopware is available in different forms. There is the free Community Edition and the [Shopware Plans](https://www.shopware.com/en/pricing/). While the plans are based on the Community Edition, they bring a variety of benefits, giving merchants and agencies the much-needed edge over the competition. As for hosting, Shopware brings, apart from self-hosting, two additional ways of hosting, each with its own benefits.

[Shopware SaaS](https://www.shopware.com/en/shopware-cloud/), hosted by Shopware, offers merchants a convenient turn-key solution with **weekly updates**.

**Shopware SaaS is always up-to-date, as we at Shopware maintain everything for you.**

With [Shopware PaaS](https://www.shopware.com/en/shopware-paas/), also hosted by Shopware, you are in charge of updating the system.

The same is true for the On-Premise version, where you download and host Shopware yourself or have someone else do it for you. In these versions, minor **releases** occur **monthly**.

If you are an extension developer or use your private extension in a cloud shop, major releases could bring the need to update your code.

These major releases in the cloud happen at the same time as the on-premise major release, to make things easier for you.

## Types of releases

There are three release types. They are named:

* Major release
* Minor release
* Patch release

The type can be inferred from the version number that is attached to a release. Shopware is using semantic versioning, with the exception of adding a "6" to the beginning, indicating it is a "Shopware 6" release in contrast to the predecessor, Shopware 5.

So in short, the version number is built like this: **6.Major.Minor.Patch**

As an example, 6.5.0.0 is a major release. The following 6.5.0.1 would be a patch release, 6.5.1.0 a minor release.

So just having a look if and which position of the version number contains zero tells you the type of release.

More on this can be read on [semver.org](https://semver.org/)
A complete overview of the current and past releases can be found at [GitHub](https://github.com/shopware/shopware/releases).

For questions on how to install a release please refer to the [documentation](https://docs.shopware.com/en/shopware-6-en/getting-started).

## Release cycles

* Minor
	* Every first Monday of the month
* Patch
	* Anytime, but only when necessary

## What effects does a release have

The different types of release are in place to indicate two things: What to expect and how big the impact in terms of work on your side is.

**Major releases** are aimed at maintaining a current and cutting-edge technical foundation, introducing substantial changes that may demand significant effort. On the other hand, **minor** and **patch** updates necessitate testing but generally do not entail disruptive breaking changes.

**Breaking changes** in Shopware refer to software modifications or updates that require developers to adjust their existing code to maintain compatibility. These changes can impact the functionality or behavior of certain features, requiring developers to update their codebase to align with the latest version of Shopware.

**Deprecations**, involve signaling that a particular feature or method is no longer recommended for use in future versions of Shopware. While deprecated features are still functional in the current version, they are marked for removal in subsequent releases. Developers are encouraged to migrate to alternative solutions or updated methods to ensure long-term compatibility and avoid potential issues when upgrading to newer versions of the software. Deprecation notices serve as a proactive way for developers to stay informed about changes and plan for the necessary updates in their projects.

### Major releases

The Major release, being the least frequent type of release delivers the most significant impact in terms of updating technical foundations, and occasionally introduces new features and architectural changes that enable Shopware to maintain a competitive edge. The effort required for adaptation depends on the level of customization in your shop and the number of extensions you use. 

Adapting Shopware to changes in the ecosystem requires implementing breaking changes. This involves adjusting Shopware internals to meet evolving requirements or updating underlying frameworks such as Symfony, Vue.js, and other dependencies. Remaining relevant in the ever-changing landscape of technology necessitates embracing change, and this process of adaptation may result in breaks. While efforts are made to minimize any inconvenience, we acknowledge that once a year, we take a significant stride toward the future. At least in parts.

Each Major Release is accompanied by a **Release Candidate (RC)**, which is typically made available approximately two months before the scheduled major release. This RC serves as an opportunity for the community to adapt, explore the changes, and provide valuable feedback.

Depending on the feedback the community gives us during the RC phase, it might be prolonged.

### Minor releases

Minor releases can be installed seamlessly without requiring modifications to extensions. These updates encompass all changes implemented in Shopware Cloud since the last minor release for **self-hosted**.

Minor releases primarily focus on the addition of features, improved functionality, or addressing minor and fringe bugs. Although the impact on extension developers is minimal in terms of required work, the benefits for merchants and agencies can be substantial. Despite the absence of breaking changes in this release type, it still introduces new features and significant improvements.

### Patch and security releases

Patch releases can be installed without the need for changes to extensions.

Given the broad array of scenarios Shopware is deployed in, there are some we can't predict or prepare for. If such a scenario occurs and the underlying code needs to be patched, we release the fix as soon as possible. As these releases are immediate and without notice, they only include important and urgent changes to Shopware. In rare cases there can be breaking changes, but only if any other measures would pose a risk to merchants.

A special kind of Patch is a release containing a security fix. These releases are usually small and contain only the fix itself, with some exceptions. These releases must be implemented as soon as possible to keep your shop and customers save.

*Please note: if updating is not possible for whatever reason, there is the security plugin which implements all security patches. It is, however, preferable to update, since patching code through a plugin can potentially cause side effects.*

<hr />

<div class="text-center">
    <p>Go download the latest Shopware version here</p>
    <a href="https://www.shopware.com/en/changelog/" class="btn">Shopware 6 Changelog</a>
</div>
