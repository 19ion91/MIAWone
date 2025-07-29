<html> 
  <body>
    <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'it'; // For example, enter 'en' or 'en-US'
			window.addEventListener("onEmbeddedMessagingConversationClosed", () => {
			    console.log("Conversation was closed!");
			});

			embeddedservice_bootstrap.init(
				'00D2o000000i2oh',
				'miaoone',
				'https://d2o000000i2oheaa-dev-ed.develop.my.site.com/ESWmiaoone1753792726519',
				{
					scrt2URL: 'https://d2o000000i2oheaa-dev-ed.develop.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://d2o000000i2oheaa-dev-ed.develop.my.site.com/ESWmiaoone1753792726519/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>


  </body>
</html>
