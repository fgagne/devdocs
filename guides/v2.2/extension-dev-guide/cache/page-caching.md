---
group: php-developer-guide
subgroup: 09_Full page caching
title: Page caching
menu_title: Full page caching
menu_order: 16
menu_node: parent
redirect_from:
  - /guides/v2.1/config-guide/cache/cache-priv-over.html
  - /guides/v2.2/config-guide/cache/cache-priv-over.html
---

{% include cache/page-cache-overview.md%}

{: .bs-callout .bs-callout-info }
Only HTTP [GET](https://www.w3.org/Protocols/rfc2616/rfc2616-sec9.html#sec9.3){:target="_blank} and [HEAD](https://www.w3.org/Protocols/rfc2616/rfc2616-sec9.html#sec9.4){:target="_blank"} requests are cacheable. For more information about caching, see [RFC-2616 section 13](https://www.w3.org/Protocols/rfc2616/rfc2616-sec13.html){:target="_blank}.
