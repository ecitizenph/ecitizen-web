<template>
	<div class="px-4 py-4 flex justify-between">
		<h1 class="text-xl text-gray-600 font-bold">Hi {{ name }}</h1>
		<div class="flex-col">
			<p class="text-right">{{ currentDate }}</p>
			<p class="text-right">{{ currentTime }}</p>
		</div>
	</div>
	<div>
		<select class="border w-full py-2 px-2 pr-8">
			<option value="">I want to apply for</option>
		</select>
	</div>
	<div class="grid grid-cols-2 gap-2 mt-8">
		<div class="bg-red-500 text-white p-8 flex items-end">
			<div>
				<svg
					xmlns="http://www.w3.org/2000/svg"
					fill="none"
					viewBox="0 0 24 24"
					stroke-width="1.5"
					stroke="currentColor"
					class="w-16 h-16"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M8.25 18.75a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m3 0h6m-9 0H3.375a1.125 1.125 0 01-1.125-1.125V14.25m17.25 4.5a1.5 1.5 0 01-3 0m3 0a1.5 1.5 0 00-3 0m3 0h1.125c.621 0 1.129-.504 1.09-1.124a17.902 17.902 0 00-3.213-9.193 2.056 2.056 0 00-1.58-.86H14.25M16.5 18.75h-2.25m0-11.177v-.958c0-.568-.422-1.048-.987-1.106a48.554 48.554 0 00-10.026 0 1.106 1.106 0 00-.987 1.106v7.635m12-6.677v6.677m0 4.5v-4.5m0 0h-12"
					/>
				</svg>

				<h2>Emergency</h2>
			</div>
		</div>

		<div class="grid gap-2">
			<div class="bg-yellow-500 p-8 text-white">
				<div>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-10 h-10"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M15.362 5.214A8.252 8.252 0 0112 21 8.25 8.25 0 016.038 7.048 8.287 8.287 0 009 9.6a8.983 8.983 0 013.361-6.867 8.21 8.21 0 003 2.48z"
						/>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M12 18a3.75 3.75 0 00.495-7.467 5.99 5.99 0 00-1.925 3.546 5.974 5.974 0 01-2.133-1A3.75 3.75 0 0012 18z"
						/>
					</svg>
					<h2 class="text-left">Report a disaster</h2>
				</div>
			</div>
			<div class="bg-green-500 p-8 text-white">
				<div>
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-10 h-10"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M17.982 18.725A7.488 7.488 0 0012 15.75a7.488 7.488 0 00-5.982 2.975m11.963 0a9 9 0 10-11.963 0m11.963 0A8.966 8.966 0 0112 21a8.966 8.966 0 01-5.982-2.275M15 9.75a3 3 0 11-6 0 3 3 0 016 0z"
						/>
					</svg>

					<h2 class="text-left">Report a crime</h2>
				</div>
			</div>
		</div>
		<div class="col-span-2">
			<div class="bg-blue-500 p-8 py-4 text-white">
				<div class="flex items-end gap-4">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-8 h-8"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 012.25-2.25h13.5A2.25 2.25 0 0121 7.5v11.25m-18 0A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75m-18 0v-7.5A2.25 2.25 0 015.25 9h13.5A2.25 2.25 0 0121 11.25v7.5m-9-6h.008v.008H12v-.008zM12 15h.008v.008H12V15zm0 2.25h.008v.008H12v-.008zM9.75 15h.008v.008H9.75V15zm0 2.25h.008v.008H9.75v-.008zM7.5 15h.008v.008H7.5V15zm0 2.25h.008v.008H7.5v-.008zm6.75-4.5h.008v.008h-.008v-.008zm0 2.25h.008v.008h-.008V15zm0 2.25h.008v.008h-.008v-.008zm2.25-4.5h.008v.008H16.5v-.008zm0 2.25h.008v.008H16.5V15z"
						/>
					</svg>

					<h2 class="text-left">Book for appointments</h2>
				</div>
			</div>
		</div>
		<div>
			<div class="bg-purple-500 p-8 py-4 text-white">
				<h2 class="text-center">LGU Profile</h2>
			</div>
		</div>
		<div>
			<div class="bg-cyan-500 p-8 py-4 text-white">
				<h2 class="text-center">LGU Directory</h2>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "HomeView",
	components: {},
	data: () => ({
		name: "Freddie Siao",
		currentDate: "0000-00-0000",
		currentTime: "00:00",
	}),

	created() {
		setInterval(this.getDate, 1000);
	},

	methods: {
		getDate() {
			const date = new Date();

			let day = date.getDate();
			let month = date.getMonth() + 1;
			let year = date.getFullYear();
			const time =
				date.getHours() + ":" + date.getMinutes() + ":" + date.getSeconds();

			this.currentDate = month + " " + day + " " + year;
			this.currentTime = time;
		},
	},
};
</script>
