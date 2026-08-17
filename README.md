$url = "https://dl.google.com/chrome/install/GoogleChromeStandaloneEnterprise64.msi"
$output = "C:\Users\Public\Downloads\ChromeSetup.msi"
(New-Object System.Net.WebClient).DownloadFile($url, $output)
