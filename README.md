# Wyrd keyword templates

Ready-made address-bar keywords for **[Wyrd](https://wyrd.page)**, the Chrome extension (some say plugin) that opens a page, a search or a record from one short keyword: type `>`, a space and the keyword in Chrome's address bar.

This repository holds the same templates [wyrd.page](https://wyrd.page) publishes, as plain files you can copy, fill in and share.

## Open a record by its number

One keyword per tool. Each address has `%s` where the words you type go. **CAPITALS are your own part of the address**: your company's Jira, your store, your repository.

| Tool | Keyword | Address | You type |
|---|---|---|---|
| [Jira](https://wyrd.page/guides/open-jira-tickets-from-the-address-bar/) | `jira` | `https://YOURCOMPANY.atlassian.net/browse/%s` | `> jira WEB-4182` |
|  | `web` | `https://YOURCOMPANY.atlassian.net/browse/WEB-%s` | `> web 4182` |
| [GitHub](https://wyrd.page/guides/open-github-issues-by-number/) | `issue` | `https://github.com/OWNER/REPO/issues/%s` | `> issue 482` |
|  | `pr` | `https://github.com/OWNER/REPO/pull/%s` | `> pr 497` |
|  | `issues` | `https://github.com/OWNER/REPO/issues?q=%s` | `> issues is:open label:bug` |
| [Azure DevOps](https://wyrd.page/guides/open-azure-devops-work-items-by-id/) | `wi` | `https://dev.azure.com/ORG/PROJECT/_workitems/edit/%s` | `> wi 4182` |
| [ServiceNow](https://wyrd.page/guides/open-servicenow-incidents-by-number/) | `inc` | `https://YOURCOMPANY.service-now.com/incident.do?sysparm_query=number=%s` | `> inc INC0012345` |
|  | `ritm` | `https://YOURCOMPANY.service-now.com/sc_req_item.do?sysparm_query=number=%s` | `> ritm RITM0010042` |
| [Zendesk](https://wyrd.page/guides/open-zendesk-tickets-by-id/) | `zd` | `https://YOURCOMPANY.zendesk.com/agent/tickets/%s` | `> zd 29101` |
|  | `zduser` | `https://YOURCOMPANY.zendesk.com/agent/users/%s` | `> zduser 3810294` |
| [Salesforce](https://wyrd.page/guides/open-salesforce-records-by-id/) | `sf` | `https://YOURCOMPANY.lightning.force.com/lightning/r/Account/%s/view` | `> sf 0015g00000XyZ12` |
|  | `opp` | `https://YOURCOMPANY.lightning.force.com/lightning/r/Opportunity/%s/view` | `> opp 0065g00000AbC34` |
|  | `sfid` | `https://YOURCOMPANY.lightning.force.com/lightning/r/%s/view` | `> sfid 0035g00000Qrs56` |
| [HubSpot](https://wyrd.page/guides/open-hubspot-records-from-the-address-bar/) | `hs` | `https://app.hubspot.com/contacts/HUB_ID/objects/0-1/views/all/list?query=%s` | `> hs maya@northwind.example` |
|  | `deal` | `https://app.hubspot.com/contacts/HUB_ID/record/0-3/%s` | `> deal 15865742643` |
| [Stripe](https://wyrd.page/guides/open-stripe-payments-by-id/) | `pay` | `https://dashboard.stripe.com/payments/%s` | `> pay pi_3Q1x7bLkdIwHu7ix` |
|  | `cus` | `https://dashboard.stripe.com/customers/%s` | `> cus cus_Q8n2…` |
| [Shopify](https://wyrd.page/guides/open-shopify-orders-by-number/) | `order` | `https://admin.shopify.com/store/STORE/orders?query=%s` | `> order 10492` |
|  | `customer` | `https://admin.shopify.com/store/STORE/customers?query=%s` | `> customer maya@northwind.example` |
| [Parcel tracking](https://wyrd.page/guides/track-a-parcel-from-the-address-bar/) | `ups` | `https://www.ups.com/track?loc=en_US&tracknum=%s` | `> ups 1Z999AA10123456784` |
|  | `fedex` | `https://www.fedex.com/fedextrack/?trknbr=%s` | `> fedex 748912345678` |
|  | `usps` | `https://tools.usps.com/go/TrackConfirmAction?tLabels=%s` | `> usps 9400100000000000000000` |

Each tool has a step-by-step guide (linked in the table) that writes the address for you and adds it to Wyrd in one click. The same rows, ready to import: [workflows/](workflows/).

## Keyword templates

Sets of keywords for a household, a small team and teams in a larger company:

- **[Everyday searches](https://wyrd.page/templates/everyday/)**: Web, videos, an encyclopedia, maps and code, each one word away. [pack (JSON)](templates/wyrd-everyday-starter-pack.json)
- **[Families and households](https://wyrd.page/templates/family/)**: School, bins, bills, the doctor and the family recipes, the same for everyone at home. [pack (JSON)](templates/wyrd-family-pack.json) · [list (CSV)](templates/wyrd-family-list.csv)
- **[Small teams](https://wyrd.page/templates/small-team/)**: Handbook, roadmap, stand-up, tickets by number and the wiki, shared by the whole team. [pack (JSON)](templates/wyrd-small-team-pack.json) · [list (CSV)](templates/wyrd-small-team-list.csv)
- **[IT admins](https://wyrd.page/templates/it-admins/)**: Admin consoles, CVE and DNS look-ups, tickets by number and runbooks, plus rollout by Chrome policy. [pack (JSON)](templates/wyrd-it-admins-pack.json) · [list (CSV)](templates/wyrd-it-admins-list.csv)
- **[HR and People teams](https://wyrd.page/templates/hr/)**: Leave, payroll, benefits, the handbook, the directory and hiring, for HR and for everyone. [pack (JSON)](templates/wyrd-hr-pack.json) · [list (CSV)](templates/wyrd-hr-list.csv)
- **[Marketing teams](https://wyrd.page/templates/marketing/)**: Analytics, ads, social, the content calendar, brand assets and a UTM builder. [pack (JSON)](templates/wyrd-marketing-pack.json) · [list (CSV)](templates/wyrd-marketing-list.csv)
- **[Teams in a larger company](https://wyrd.page/templates/enterprise-teams/)**: Stand-up, board, roadmap and on-call for one team, layered on the company-wide list. [pack (JSON)](templates/wyrd-enterprise-teams-pack.json) · [list (CSV)](templates/wyrd-enterprise-teams-list.csv)

## How to use them

1. **Install Wyrd:** [Chrome Web Store](https://chromewebstore.google.com/detail/wyrd/jpoppmijoimaipaibckkkibejgohjmdn). Free, no account.
2. **Load a template:** open its page on wyrd.page and press **Load in Wyrd**, or import a CSV here in Wyrd's **Keyword tools → Import**. Fill in the addresses marked as yours before you save them.
3. **Share them with a team:** copy a CSV into your own Google Sheet or GitHub repository, change the CAPITALS to your addresses, and have everyone subscribe to it in Wyrd's **Shared lists**. When an address changes, change it once there. Guide: [share links with your team](https://wyrd.page/guides/share-links-with-your-team/).

The files are Wyrd's list format: `Keyword, URL, Description, Category`, one keyword a row. Rows starting with `!` set the list's name and short name.

## About

Made by the makers of Wyrd. Questions or a tool you would like here: hello@wyrd.page. More guides: https://wyrd.page/guides/.
