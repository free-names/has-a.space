<h1 align="center">has-a.space</h1>

<p align="center"><strong>has-a.space</strong> is a free subdomain service made by <a href="https://github.com/doughmination">Clove Twilight</a></p>
<br>
<p align="center">
   <a href="https://discord.gg/aVzSvXCy5v"><img alt="Discord Server" src="https://inv.doughmination.gay/?inviteCode=aVzSvXCy5v"></a>
</p>

> [!WARNING]
> We do not support Vercel at the moment since we are not on the PSL.

## Issues
If you have any problems, feel free to [open an issue](https://github.com/free-names/has-a.space/issues/new/choose).

Please follow our ToS, which can be found [here](https://free-names.org/terms)

## Register
1. Fork [the repository](https://github.com/free-names/has-a.space/fork).
2. Make a json file in the `domains` directory, for example `example.json`.
3. Add the following file format to the json you just made:
```json
{
    "owner": {
        "username": "your-github-username",
        "email": "hello@example.com",
        "repo": "your-website's-repository-link-here"
    },

    "records": {
        "A": ["1.1.1.1", "1.0.0.1"],
        "AAAA": ["2606:4700:4700::1111", "2606:4700:4700::1001"],
        "CNAME": "example.com",
        "MX": ["mx1.example.com", "mx2.example.com"],
        "TXT": ["example_verification=1234567890"],
        "NS": ["ns1.example.com", "ns2.example.com"],
        "SRV": [
            { "priority": 10, "weight": 60, "port": 5060, "target": "sipserver.example.com" },
            { "priority": 20, "weight": 10, "port": 5061, "target": "sipbackup.example.com" }
        ],
        "DS": [
            {
                "key_tag": 2371,
                "algorithm": 13,
                "digest_type": 2,
                "digest": "...."
            }
        ]
    },
    "proxied": false
}
```
> [!NOTE]
> Only select the records you need, this is just an example of all the records we support.

4. Make a pull request to the repo and wait for it to be merged, if you don't know how to make a pull request please read [GitHub's guide](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
5. After the pull request is merged, the DNS records should propagate within the next 15-20 minutes, however in rarer cases, it can sometimes takes between 24-48 hours.
6. That's all, enjoy your `has-a.space` subdomain!

> [!NOTE]
> If your DNS has not propagated within 48 hours, please check with a [DNS Checker](https://dnschecker.org/all-dns-records-of-domain.php) before contacting us, so we can get you the best support.

## Documentation
Our documentation is available [here](https://docs.free-names.org)!

### Similar Services
If you want to find services that are similar to has-a.space, please check out [Open Domains](https://github.com/open-domains/register), [is-a.dev](https://github.com/is-a-dev/register), [part-of.my.id](https://github.com/partofmyid/register), [is-not.cool](https://github.com/is-not-cool/registration) and any other subdomain provider available to the world.
