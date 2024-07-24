# rawGitHubFetcher
for fetching small files from raw.githubusercontent.com ... even from  🇨🇳


## Usage example

```
byte[] data = Fetcher.get("https://raw.githubusercontent.com/psilo-hub/rawGitHubFetcher/main/README.md");
System.out.println(data==null?"null":new String(data, StandardCharsets.UTF_8));
```