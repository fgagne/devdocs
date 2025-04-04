---
group: architecture-guide
title: Ease of frontend customization
menu_title: Ease of frontend customization
redirect_from:
- guides/v2.1/architecture/storefront_customization.html
---

## Overview {#m2arch-whatis-overview}

The Magento [frontend](https://glossary.magento.com/frontend) is designed to optimize [storefront](https://glossary.magento.com/storefront) customization, with highly extensible *themes* being the central customization mechanism.

Merchants are encouraged to use Magento components and themes to extend and transform the appearance of their storefronts.

## Storefront customization tools

Magento provides several tools to help you significantly jumpstart the storefront customization process:

* Magento Blank [Theme](https://glossary.magento.com/theme)

* [Magento UI Library Components][]

* [Magento Admin Pattern Library][]

See the [Frontend Developer Guide][] for information on creating your themes.

### Magento Blank theme

The Magento blank theme template provides a launchpad for storefront customization. You can use this boilerplate as a robust starting point for your own theme development.

### Magento UI components

Using Magento standard coding and styling tools can help:

* enforce for consistency in design across your storefronts
* simplify (and speed up) the design process

This component [library](https://glossary.magento.com/library) contains standard reusable components for form features, such as fields and buttons, and navigation elements. The Magento UI library is a set of generic web components and Magento-specific patterns, which simplifies the process of Magento theme creation and customization.

See [Magento UI Library Components][] for details about this library.

### Magento Admin pattern library

A *pattern library* is a collection of user interface (UI) design patterns that can be re-used in locations throughout your product installation. The [Magento Admin Pattern Library][] defines examples of components that administrators working with the storefront can use.

Form elements included in the [Magento Admin](https://glossary.magento.com/magento-admin) pattern library include:

* address form
* button bar
* container
* tabs
* sign-in form

Users of the default Magento storefront encounter examples of these form elements throughout the product. These patterns provide a valuable language of software components (and indirectly, user experiences) for [extension](https://glossary.magento.com/extension) developers and administrators.

The Magento [Admin](https://glossary.magento.com/admin) Pattern library is built on the Less preprocessor and implemented as a [module](https://glossary.magento.com/module). You can download a free, current version of this module from [Magento Marketplace](https://marketplace.magento.com/).

See [Magento Admin Pattern Library][] for more information on using this library.

### Storefront customization levels

These four levels of potential storefront customization are listed in order to increase complexity.

#### Extend Magento-Provided CSS

Magento supplies a default {% glossarytooltip d2093e4a-2b71-48a3-99b7-b32af7158019 %}theme{% endglossarytooltip %} and a Less-based CSS. You can substantially change a storefront using CSS only. This uncomplicated strategy might suit projects with a limited budget, or might interest developers who create different skins for a site. A small business enter this process of storefront customization by buying a third-party developed theme from Magento Marketplace to extend the default values.

#### Replace PHTML template files

In addition to extending the default CSS, you can generate different HTML {% glossarytooltip 8f407f13-4350-449b-9dc5-217dcf01bc42 %}markup{% endglossarytooltip %}. For example, you might need to add a missing CSS class name, or an add an extra `<div>` tag to achieve some visual effect. You might also need to tweak some {% glossarytooltip 312b4baf-15f7-4968-944e-c814d53de218 %}JavaScript{% endglossarytooltip %} to cope with different HTML markup. This change is more demanding than simply extending Magento CSS, but is still within the grasp of smaller projects and leaner teams.

#### Replace Magento-Provided CSS

Rather than edit the default CSS provided by Magento, you might decide to replace all the default storefront CSS code with your own. This strategy avoids tying a project to the Magento-provided CSS, but puts a greater burden on project development and integration. It also allows use of different CSS tools or technologies not provided with Magento. Partners who build their own set of CSS libraries could reuse these libraries on different customer projects. (These unique CSS libraries may help differentiate a partner from others in the market.)

In addition to replacing CSS files, you might need to replace small amounts of HTML and JavaScript.

#### Replace Magento-Provided CSS, HTML, and JavaScript

Delivering a sharply different shopping experience than the default Magento installation provides is a more substantial task. However, the tradeoff might be a more complicated experience integrating additional extensions into your installation in the future.

{:.bs-callout .bs-callout-tip}
 Any customization of your storefront will work optimally, and provide the easiest path for later upgrades, if you follow the best practice of consistently compartmentalizing code by type. For example, keep all HTML in {% glossarytooltip ae0f1f68-c466-4189-88fd-6cd8b23c804f %}PHTML{% endglossarytooltip %} files; keep all JavaScript in JavaScript files.

## Related topics {#m2arch-related}

[Extensibility and modularity][]

[Global extensibility features][]

[Magento Admin Pattern Library][]

[Magento UI Library Components][]

<!-- Link definitions-->

[Magento Admin Pattern Library]: {{page.baseurl}}/pattern-library/bk-pattern.html
[Magento Marketplace]: https://marketplace.magento.com/
[Magento UI Library Components]: {{page.baseurl}}/ui-components/ui-component.html
[Frontend Developer Guide]: {{page.baseurl}}/frontend-dev-guide/bk-frontend-dev-guide.html
[Extensibility and modularity]: {{page.baseurl}}/architecture/extensibility.html
[Global extensibility features]: {{page.baseurl}}/architecture/global_extensibility_features.html