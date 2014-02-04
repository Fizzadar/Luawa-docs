Lhtml is the templating language Luawa uses.

<div class="pre-filename">request.lua</div>

	template:set( 'messages', {{ type = 'success', text = 'hello world' }})
	template:load( 'hello-world' )	

<div class="pre-filename">hello-world.lhtml</div>

	<div>
		<? for k, message in pairs( self:get( 'messages' )) do ?>
			<div class="message <?=message.type ?>">
				<?=message.text ?>
			</div>
		<? end ?>
	</div>
