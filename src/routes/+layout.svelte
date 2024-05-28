<script>
	import '../app.css';
</script>

<div class="text-sm max-w-[600px] mx-auto mt-6 flex flex-row justify-between">
	<a href="/" class="hover:underline">Aeron Laffere</a>
	<ul class="flex flex-row gap-2">
		<li><a href="/about" class="underline text-blue-600">about</a></li>
		<li><a href="/" class="underline text-blue-600">blog</a></li>
		<li><a href="/bookmarks" class="underline text-blue-600">bookmarks</a></li>
	</ul>

</div>
<div class="max-w-[600px] mx-auto mt-16 text-sm">
<slot></slot>
</div>


<style></style>
