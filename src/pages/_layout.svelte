<div class="container py-3">
	<h1 class="text-center">Buku Aqidah</h1>
	<hr>
	<div class="row">
		<div class="col-sm-3 mb-3">
			<div class="list-group">
				<div class="list-group-item"><strong>Daftar Isi</strong></div>
				{#each daftarIsi as x}
					<a href="/{x.link}" class="list-group-item list-group-item-action">{x.judul}</a>
				{/each}
			</div>
		</div>
		<div class="col-sm mb-3">
			<slot></slot>
		</div>
	</div>
</div>

<script>
	const daftarIsi = [
		{link: '', judul: 'Beranda'},
		{link: 'pertama', judul: 'Pertama'},
		{link: 'tentang-penulis', judul: 'Tentang Penulis'}
	]
</script>