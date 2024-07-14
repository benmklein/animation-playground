<script lang="ts">
	let hover = false;
</script>

<div class="box-border h-screen bg-gradient-to-b from-gray-700 to-gray-800 p-4">
	<div class="container m-auto h-full rounded-3xl border border-gray-800 shadow-lg shadow-gray-950">
		<div
			class="flex h-full flex-row gap-2 rounded-3xl bg-gradient-to-br from-neutral-950 to-neutral-900"
		>
			<div
				class="basis-1/6 rounded-l-3xl border-r border-r-gray-800 bg-neutral-950 p-4 text-gray-100"
			>
				Side bar
			</div>
			<div class="flex basis-5/6 flex-col gap-4">
				<div class="basis-1/6 p-4 text-gray-100">Top bar</div>
				<div class="flex h-full flex-row gap-4 p-8">
					<div class="flex basis-3/4 flex-col gap-4">
						<div
							class:hover
							on:mouseenter={() => {
								hover = true;
							}}
							on:mouseleave={() => {
								hover = false;
							}}
							class="basis-1/6 rounded-xl bg-neutral-900 shadow-inner shadow-neutral-800"
						>
							Animating text
						</div>
						<div class="basis-3/6 rounded-xl bg-cyan-950 shadow-inner shadow-cyan-800"></div>
						<div class="mb-2 basis-2/6 rounded-xl bg-cyan-950 shadow-inner shadow-cyan-800"></div>
					</div>
					<div
						class="mb-2 mr-2 basis-1/4 rounded-xl bg-cyan-950 shadow-inner shadow-cyan-800"
					></div>
				</div>
			</div>
		</div>
	</div>
</div>

<style lang="postcss">
	.hover {
		color: theme(textColor.pink.500);
	}
</style>
