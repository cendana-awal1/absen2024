<script>
	export let item;
</script>

<!-- Card Student -->
<div class="flex flex-col items-center justify-center w-64 h-96 bg-white rounded-lg shadow-lg p-6 dark:bg-surface-dark dark:shadow-gray-600">
  <img class="w-24 h-24  rounded-full mx-auto mb-4 image" src="https://drive.google.com/thumbnail?id={item.foto}" alt="Student">

  <div class="w-24 h-24 mx-auto mb-4">
    <img
					src="https://api.qrserver.com/v1/create-qr-code/?data={item.nama}&amp;size=120x120"
					alt={item.nama}
				/>
  </div>

  <h3 class="text-lg font-medium text-gray-900 dark:text-white">{item.nama}</h3>
  <button class="w-full bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
    {item.Kelas}
  </button>
</div>

