# TR BTC-ETH-main

## Details

Repo assoicated with TraderTraitor and "Verity Stroud"

Taken from https://github.com/ashish6976/BTC-ETH on Aug 27 2024

Archive: https://archive.ph/AHYS7

Archive of `price.py`: https://archive.ph/6AVOM

See also: https://x.com/tayvano_/status/1810455262320570416

See also: [Coinstats](../hacks-and-thefts/coinstats.md)


## Inside the repo

There are a whopping total of 3 files:

1. requirements.txt which has a whopping total of 2 lines: `pyyaml` and `requests`

2. README.md which has a whopping total of 2 lines: `pip3 install -r requirements.txt` -> `python3 price.py`

3. `price.py` which has a whopping total of 100 lines


### price.py

Given the simplicity of the codebase, the lack of malicious/compromised PyPi packages, and the lack of post-install scripts, the insert must come from a malicious c2 api endpoint.

The code for processing the data the API endpoints is:

```
if content_type.startswith("application/json"):
    return json.loads(resp.text)

elif content_type.startswith("application/x-www-form-urlencoded"):
    return parse_qs(resp.text)

elif content_type.startswith("application/yaml"):
    return yaml.load(resp.text, Loader=yaml.Loader)
```

There is no validation really on anything any api returns. it does ignore and continue to run if given any errors.

The legitimate API endpoints returns `application/json`

Presumably the malicious URL will return something else, most likely a malicious YAML. Because there's really no reason to load pyyaml in the first place for such a simple codebase.

And because:

> Loading untrusted YAML can lead to arbitrary code execution due to deserialization vulnerabilities. Because `yaml.load(resp.text, Loader=yaml.Loader)` directly loads the YAML content into the program’s memory, if the malicious server sends a YAML file containing Python objects or instructions, it could trigger remote code execution on the user's device. Always use `yaml.safe_load()` instead of `yaml.load()` to avoid deserialization of arbitrary objects in YAML data.

See also: https://security.gentoo.org/glsa/202402-33


### C2s

There are 2 confirmed variations: one using `coinhar[.]io` and one with `indobit[.]io`

e.g. `for company in ["Binance", "Kucoin", "Wazirx", "Coinhar", "Indodax"]`

- Binance endpoint: `https://api.binance.com/api/v3/ticker/price?symbol=ETHBTC`

- Kucoin endpoint: `https://api.kucoin.com/api/v1/market/stats?symbol=ETH-BTC`

- Wazirx endpoint: `https://api.wazirx.com/sapi/v1/ticker/24hr?symbol=ethbtc`

- Coinhar [sic] endpoint: `https://api.coinhar.io/api/v3/ticker?symbol=ETHBTC`

- Indodax: `https://indodax.com/api/ticker/ethidr`

- Indodax: `https://indodax.com/api/ticker/btcidr`

Previously, coinhar was indobit:

- indobit [sic] endpoint: `https://api.indobit.io/api/v3/ticker?symbol=ETHBTC`


#### "Coinhar"

- https://www.virustotal.com/gui/domain/coinhar.io/relations

- https://search.censys.io/hosts/185.62.58.122

- 2024-03-29

- `api.coinhar[.]io`

- `185.62.58[.]122`

- Snel.com, NL

- Reverse DNS bastion01.eu-west-03.hoolia.eu

- 22/SSH, 445/SMB, 8080/HTTP


#### Indobit

- https://www.virustotal.com/gui/domain/indobit.io/relations

- https://www.virustotal.com/gui/ip-address/146.70.88.126

- 2024-03-22 `api.indobit[.]io`

- 2024-03-20 3/94 `146.70.88[.]126`

- M247 Europe SRL

- 22/SSH


# MALICIOUS SHIT INCOMING 

🚨🚨🚨🚨🚨🚨🚨🚨🚨

🚨🚨🚨🚨🚨🚨🚨🚨🚨

**[Malicious repo](./TR_MALICIOUS_BTC-ETH-main.zip)**

(zip is fine, running will rekt you. Don't do it!)

🚨🚨🚨🚨🚨🚨🚨🚨🚨

🚨🚨🚨🚨🚨🚨🚨🚨🚨