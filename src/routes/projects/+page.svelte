<script lang="ts">
    import mouse from '$lib/assets/projects/wire_frame_laboratory_mouse.png'
    import eeg from '$lib/assets/projects/wire_frame_eeg_cap.png'
    const data = [
        {
            title: 'The role of striatal dopamine release in long-term learning',
            description: 'This is a project description',
            start: '2020',
            end: '2023',
            image: mouse
        },
        {
            title: 'Auditory attention and synchronous brain activity',
            description: 'This is a project description',
            start: '2016',
            end: '2019',
            image: eeg
        },
        {
            title: 'Psychometric identification of UAS pilot suitability',
            description: 'This is a project description',
            start: '2024',
            end: '',
            image: ''
        },
        {
            title: 'Neuronal architecture of predictive coding',
            description: 'This is a project description',
            start: '2017',
            end: '2019',
            image: ''
        },
        {
            title: 'Dopamine and long-term learning',
            description: 'This is a project description',
            start: '2020',
            end: '2023',
            image: ''
        },   
    ]
</script>
<div class="grid grid-cols-2 lg:grid-cols-3 md:gap-12 gap-4">
    {#each data as { title, description, start, end, image }}
        <div class="border h-[500px] p-4 rounded flex flex-col  justify-between gap-y-2 cursor-pointer md:opacity-90 hover:opacity-100 hover:border-gray-300 hover:shadow-sm transition-all duration-300">
            <div class="flex flex-col gap-y-2">
            <p class="text-xs text-gray-500">{start} — {end}</p>
            <h3 class="text-lg">{title}</h3>
            <p>{description}</p>
        </div>
            <img src={image} alt={title} class="w-full h-48 object-cover" />
        </div>
    {/each}
</div>