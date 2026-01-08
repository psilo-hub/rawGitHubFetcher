# rawGitHubFetcher

for fetching small files from raw.githubusercontent.com ... even from  🇨🇳


## Usage example

```
byte[] data = Fetcher.get("https://raw.githubusercontent.com/psilo-hub/rawGitHubFetcher/main/README.md");
System.out.println(data==null?"null":new String(data, StandardCharsets.UTF_8));
```

## Background

Back when ChatGPT was the only LLM that was kind of free and useful I found a [GitHub repo](https://github.com/LiLittleCat/awesome-free-chatgpt) that offered a frequently updated list of "mirror" sites as the OpenAI pages were (and still are) blocked in 🇨🇳.

So I made an Android app that would fetch that list, test connectivity and open a page that seemed to be working. As the connectivity to GitHub is also flaky in 🇨🇳 I wrote this little module to fetch the list.

Now there's [DeepSeek](https://chat.deepseek.com/) and that mirror list doesn't get updated anymore, but still this tiny fetcher might be useful to some.