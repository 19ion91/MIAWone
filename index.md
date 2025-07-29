<html> 
	<head><link rel="icon" href="data:,"></head>
  <body>
    <script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'it'; // For example, enter 'en' or 'en-US'
			window.addEventListener("onEmbeddedMessagingConversationClosed", e => {

                        	console.log("Received the onEmbeddedMessagingConversationClosed event…");

                        	const footer = document.querySelector("embeddedmessaging-input-footer");
  if (footer) {
  console.log("footer found");
    footer.style.display = "none";
  } else {
  console.log("footerItemsContainer1 NOT found");
}

  const footer1 = document.querySelector(".footerItemsContainer");
if (footer1) {
  console.log("footerItemsContainer found");
  footer1.style.display = "none";
} else {
  console.log("footerItemsContainer2 NOT found");
}

const footer2 = document.querySelector(".embeddedMessagingInputTextAreaWrapper");
if (footer2) {
  console.log("embeddedMessagingInputTextAreaWrapper found");
  footer2.style.display = "none";
} else {
  console.log("footerItemsContainer3 NOT found");
}


 console.log("aaa");



// Step 1: Get the embedded messaging root element
  const embeddedMessaging = document.querySelector("embedded-messaging");

  if (!embeddedMessaging) {
    console.log("embedded-messaging not found");
    return;
  }

  // Step 2: Access shadow root
  const shadowRoot = embeddedMessaging.shadowRoot;
  if (!shadowRoot) {
    console.log("No shadowRoot found on embedded-messaging");
    return;
  }

  // Step 3: Look deeper if needed – sometimes it's nested further
  const conversationRoot = shadowRoot.querySelector("embeddedmessaging-conversation");
  if (!conversationRoot) {
    console.log("embeddedmessaging-conversation not found");
    return;
  }

  const conversationShadow = conversationRoot.shadowRoot;
  if (!conversationShadow) {
    console.log("No shadowRoot found on embeddedmessaging-conversation");
    return;
  }

  // Step 4: Find and hide the target element
  const footer = conversationShadow.querySelector(".footerItemsContainer");
  if (footer) {
    footer.style.display = "none";
    console.log("footerItemsContainer hidden");
  } else {
    console.log("footerItemsContainer not found");
  }


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
