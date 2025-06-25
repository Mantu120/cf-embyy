**A cloudflare worker script to reverse pro*xy emby**

Log into Cloudflare and create a new Worker: 
 Log into your Cloudflare account.
    Navigate to “Workers & Pages”.
    Click “Create a Service” to create a new worker service.
    Give your worker a name and select “HTTP handler”.

Write the Worker script: 
 Copy and paste the code of worker.js in the Worker editor.

Deploy Worker: 
 Save and deploy your worker. 
 Make a note of your worker's subdomain (e.g. your-worker.your-domain.workers.dev).

Configure DNS: 
 In Cloudflare's DNS settings, create a new CNAME record pointing to your Worker subdomain.
    For example, if you want to access the Emby server via emby.your-domain.com, you can create a CNAME record: 
 Name: emby 
 Target: your-worker.your-domain.workers.dev

Test: 
 Replace your Emby server address with your configured domain name (e.g., emby.your-domain.com) to confirm that the proxy function is working properly.

Translated with DeepL.com (free version)
