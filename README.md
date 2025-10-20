# `nyno-serper-search` — Simple Search for Serper for Nyno Workflows

![Nyno Log Screenshot](/h/f37d79435106d4decb25be5ab49d4d5a853922ba79d6e497f3f2255d5207d62b/screenshot-from-2025-10-15-18-12-08.webp)

## Overview

`nyno-serper-search` is a lightweight [Nyno](https://github.com/empowerd-cms/nyno)  extension to search with Serper and retrieve Google Search Results.


## 📝 YAML Usage in Nyno Workflows

Add this command to your Nyno workflow YAML:

```yaml
nyno-serper-search:
  args:
    - "${apiKey}"
    - "${search}"
```

* `${apiKey}` → Your OpenAI API key
* `${imagePath}` → Path to the image you want to edit
* `${prompt}` → Description of the desired edit

![/h/a430a14b77eb61eff79e6b3edf41decdfb160158c2612efdb3b0ab965f13574a/screenshot-from-2025-10-14-20-32-45.webp](/h/a430a14b77eb61eff79e6b3edf41decdfb160158c2612efdb3b0ab965f13574a/screenshot-from-2025-10-14-20-32-45.webp)

---

🚀 Install & Link Locally

```
git clone https://github.com/empowerd-cms/nyno-serper-search
cd nyno-serper-search
npm link # this makes the 'nyno-serper-search' command available
```

## ⚡ Execute via TCP (`tcpman`)

You can also run the Nyno workflow with the example YAML using **TCP/tcpman**:

```bash
tcpman localhost:6001/test_ai \
  'c{"apiKey":"changeme"}' \
  'q{"search": "keywords for SERP results","apiKey":"..."}'
```

* `c{...}` → Connection/authentication parameters
* `q{...}` → Query/execution parameters corresponding to YAML arguments
* Replace `keywords for SERP results` with your query
* Replace `...` with your Serper API key


## 🧾 License

Licensed under the [Apache License 2.0](./LICENSE).

