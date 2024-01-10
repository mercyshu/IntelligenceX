<div align="center">
  <h1>IntelligenceX GoLang Project</h1>
</div>
<p align="center">
   Intelligence X is a search engine and data archive. Search Tor, I2P, data leaks and the public web by email, domain, IP, CIDR, Bitcoin address and more.
</p>

To start project:

```
go mod tidy
go run main.go
```

How to use:

```go
http.ListenAndServe(":1384", Router.AppRoutes())
```
The statement starts an HTTP server and starts listening for incoming requests on the specified port. (http://localhost:1384/)

Specify a Api Key:
```go
File Location: App/Services/Applicate

const publicAPIKey = "YOUR_INTELLIGENCEX_KEY"
```

A guide for you to realize your requests:

```
SearchFileFromId        Prints file content with did.           /IntelligenceX/SearchFileFromId?Id=d453e9d5-bad0-4e5b-ac95-ae6962e143d2
SearchStart             Starts a search and returns the search ID
SearchStartAdvanced     Starts a search with optional parameters and returns the search ID
SearchGetResults        Returns available results
SearchTerminate         Terminates a search
FilePreview             Returns the preview (max first 1000 characters) of an item
FileRead                Returns the full item data
SearchGetResultsAll     Returns all results within a timeout
SetAPIKey               Sets API URL and Key to use
```
