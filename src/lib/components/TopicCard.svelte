<div class="card w-96 bg-base-100 shadow-xl">
	<div class="card-body">
		<h2 class="card-title"><slot name="title" /></h2>
		<slot name="description" />
		<div class="card-actions justify-end">
			<slot name="button" />
		</div>
	</div>
</div>
