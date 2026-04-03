# PlugPlay

### **How to Identify the Right Process** <a href="#come-identificare-il-processo-corretto" id="come-identificare-il-processo-corretto"></a>

To analyze this service, you must first locate the instance that hosts it. You can do this by searching for the "PlugPlay" service. Often, this process is also referred to as . The best strategy is to focus on the instance with the highest value of "Private Bytes", as it is more likely to be the one where code was injected.`svchost.exeDcomLaunch`

#### **How to Search for Evidence** <a href="#come-cercare-le-prove" id="come-cercare-le-prove"></a>

Once the process has been identified, the method of investigation is very targeted. You don't have to scan all files, but look specifically for file references.`.jar`

The primary search expression should be:

* Search String: `.jar`

Finding complete paths that end with within a process as or represents solid evidence of suspicious activity.`.jarPlugPlayDcomLaunch`
