# Roten (easy)

## Step 1
Analyzing the pcap file I first filtered by post requests.
`http.request.method == "POST"`
With this I found the upload of a malicious file galacticmap.php. We know this is malicious because we see some obfuscated php code and it was used to perform remote excecution.

## Step 2
This step required analysis of the code. It looks like multiple strings are placing combined and manipulated then ran through `eval`.
I figured I could just run this code however get to print out the string rather than excecute it. 
Sure enough I get the soruce code for the web shell along with the flag.