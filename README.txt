Booster Lab — Google Sites + jsDelivr

This static download runs offline gameplay only. Friend trading and its shared server
are available only in the live Booster Lab app. No credentials are included.

1. Extract this ZIP. Upload booster-lab.js, booster-lab.css, pack-images, and
   crown-card-images
   to the ROOT of a PUBLIC GitHub repository. Do not upload the ZIP itself.
2. Wait for this link to show JavaScript instead of a 404:
   https://cdn.jsdelivr.net/gh/YOUR_GITHUB_USERNAME/YOUR_PUBLIC_REPO@main/booster-lab.js
   The CDN domain is cdn.jsdelivr.net, which you confirmed works at school.
3. Open google-sites-embed.html in a text editor and replace all three occurrences
   of YOUR_GITHUB_USERNAME/YOUR_PUBLIC_REPO with your GitHub details.
4. In Google Sites, select Insert > Embed > Embed code. Paste the entire snippet,
   click Next > Insert, resize the embed to at least 900px tall, then Publish.
5. Test the published Google Site at school. Crown Zenith's 230 Collectr scans
   are bundled in crown-card-images and load from your jsDelivr-hosted repo.
   Other sets still load their scans from external catalog services.

Do not use the jsDelivr URL of an .html file as an iframe: jsDelivr serves HTML
as plain text. The Google Sites snippet loads only the JS, CSS, and images.
