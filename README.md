[![](https://images.microbadger.com/badges/image/jdrbahamut/wikimedia.svg)](http://microbadger.com/images/jdrbahamut/wikimedia "Badge provided by microbadger.com")

# What is MediaWiki?

MediaWiki is a free and open-source wiki app, used to power wiki websites such
as Wikipedia, Wiktionary and Commons, developed by the Wikimedia Foundation and
others.

> [wikipedia.org/wiki/MediaWiki](https://en.wikipedia.org/wiki/MediaWiki)

# How to use this image

    docker run --name some-mediawiki -v /local/data/images:/usr/share/nginx/html/images \ 
                                     -v /local/data/extentions_to_install:/tmp/extensions \
                                     -v /local/data/LocalSettings.php:/usr/share/nginx/html/LocalSettings.php:ro \
                                     -d jdrbahamut/mediawiki


Extensions in the /tmp/extensions folder of the images will be copy into extensions folder at the startup of the container.
