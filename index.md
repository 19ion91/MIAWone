<html> 
  <body>
    <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'it'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00D2o000000i2oh',
				'toGitHub',
				'https://d2o000000i2oheaa-dev-ed.develop.my.site.com/ESWtoGitHub1753792271545',
				{
					scrt2URL: 'https://d2o000000i2oheaa-dev-ed.develop.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://d2o000000i2oheaa-dev-ed.develop.my.site.com/ESWtoGitHub1753792271545/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

  </body>
</html>
