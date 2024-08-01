# <p align="center"> *.app-from.us.to domain </p>
**<p align="center"> Get your free `{name}.app-from.us.to` subdomain </p>**

<p align="center">
    <img src="https://img.shields.io/github/stars/thedev-me/register?label=stars&style=for-the-badge&color=FFD700" alt="GitHub stars">&nbsp;&nbsp;
    <img src="https://img.shields.io/github/directory-file-count/thedev-me/register/domains?label=domains&style=for-the-badge&color=4CAF50" alt="Domains">&nbsp;&nbsp;
    <img src="https://img.shields.io/github/issues-pr/thedev-me/register?label=Pull%20Requests&style=for-the-badge&color=FFA500" alt="GitHub pull requests">&nbsp;&nbsp;
</p>


## How to Get Your Subdomain

1. 🌟 Star and fork this repository
2. 📰 Read the entire README and review our [Terms of Service](TERMS.md)
3. 🗄️ Create a JSON file and name it `yoursubdomain.thedev.me.json` in `./domains` of your forked repo.
4. ✍️ Fill in the JSON file (format and instructions below). Make sure the JSON is valid with no trailing commas.
5. 🫷 Open a pull request with your changes.
6. 🤖 Automated checks will run and report any JSON errors. (First-time contributors await a manual trigger.)
7. ✅ After manual review and approval, your subdomain will be live within minutes.

> [!NOTE]
> Passing automated checks does NOT guarantee approval. All submissions undergo manual review to ensure quality and compliance. Read our [Terms of Service](TERMS.md).


## Supported Record Types

- We support **A, AAAA, CNAME, NS, MX, and TXT** record types.

- **We do NOT support wildcards or sub-subdomains.** <sub>(yet).</sub>

- Always **Free SSL** for own subdomains


## JSON Formatting

To register your subdomain, create a new JSON file in the `./domains` directory. The filename should be in the following format, `yoursubdomain.thedev.me.json`.

Use the following structure for your JSON file.

> [!IMPORTANT]  
> Keep only the necessary records, update their values as needed, and delete the others. Typically, this means an IP address as an A record or a hostname as a CNAME record. NS records specify the nameservers that store DNS records. MX and TXT records handle email routing and ensure email authenticity and domain ownership. [Learn more about DNS records.](https://www.cloudflare.com/learning/dns/dns-records/)

> [!IMPORTANT]
> Ensure your JSON file is valid with NO trailing commas. You can easily check the format validity [here](https://jsonlint.com).

```json
{
  "subdomain": "yoursubdomain",
  "domain": "app-from.us.to",
  "public_email": "user@example.com",
  "github_username": "user",
  "description": "A brief description of the purpose of the subdomain",

  "records": {
    "A": [
      "192.0.2.1",
      "192.0.2.2"
    ],
    "AAAA": [
      "2001:db8::1",
      "2001:db8::2"
    ],
    "CNAME": [
      "example.com"
    ],
    "NS": [
      "ns1.example.com",
      "ns2.example.com"
    ],
    "MX": [
      "mail1.example.com",
      "mail2.example.com"
    ],
    "TXT": [
      "v=spf1 include:_spf.example.com ~all"
    ]
  },
  "proxied": true
}
```


## Fields Explanation

- `subdomain`: Your desired subdomain (e.g., "myproject" for myproject.thedev.me)
- `domain`: Always "app-from.us.to"
- `public_email`: Your public contact email
- `github_username`: Your GitHub username
- `description`: A brief description of your subdomain's purpose
- `records`: DNS records for your subdomain. Only keep the ones you need. [Learn more.](https://www.cloudflare.com/learning/dns/dns-records/)
- `proxied`: Set to `true` if you want to use Cloudflare's proxy, `false` otherwise.


## Terms and Conditions

By using this service, you agree to be bound by our [Terms of Service](TERMS.md). Please review them carefully.

