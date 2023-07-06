<div class="collapse collapse-arrow bg-base-200">
	<input type="radio" name="my-accordion-2" />
	<div class="collapse-title text-xl font-medium">
		<slot name="title" />
	</div>
	<div class="collapse-content">
		<p><slot name="description" /></p>
		<p><slot name="button" /></p>
	</div>
</div>
