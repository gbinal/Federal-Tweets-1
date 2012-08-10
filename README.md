Federal-Tweets-1
================

Streaming Tweets From Across Government



Problem: How to add code to the search: ____  section to have the list of twitter accounts from either of these:
http://registry.usa.gov/accounts.json?service_id=twitter
or 
http://registry.usa.gov/accounts.xml?service_id=twitter


Initial Code: 




<script charset="utf-8" src="http://widgets.twimg.com/j/2/widget.js"></script>
<script>
new TWTR.Widget({
  version: 2,
  type: 'search',
  search: 'from:fcc OR from:usgsa OR from:epagov',
  interval: 30000,
  title: '',
  subject: 'US Government - Recent Tweets',
  width: 250,
  height: 300,
  theme: {
    shell: {
      background: '#8ec1da',
      color: '#ffffff'
    },
    tweets: {
      background: '#ffffff',
      color: '#444444',
      links: '#1985b5'
    }
  },
  features: {
    scrollbar: false,
    loop: true,
    live: true,
    behavior: 'default'
  }
}).render().start();
</script>



