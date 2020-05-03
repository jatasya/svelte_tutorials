<script>
  import MeetupItem from "./MeetUps/MeetupItem.svelte";
  import Header from "./UI/Header.svelte";
  const meetups = [
    {
      id: "m1",
      title: "Cool Meetup 1",
      subtitle: "Cool Meetup subtitle 1",
      description: "Cool Meetup 1",
      imageUrl:
        "http://upload.wikimedia.org/wikipedia/commons/8/86/King_Eider_%28Somateria_spectabilis%29_%2813667616745%29.jpg",
      address: "Bangalore 1",
      contactEmail: "cool@meetup1.com"
    },
    {
      id: "m2",
      title: "Cool Meetup 2",
      subtitle: "Cool Meetup subtitle 2",
      description: "Cool Meetup 2",
      imageUrl:
        "https://lh6.ggpht.com/L7Uu4h1AkGk_P3pejv-FQfTaRDXl9T9VTJCP8aXpqsZaChMh_TwmrBXkn6g5ZjFfsSc=h900",
      contactEmail: "cool@meetup2.com",
      address: "Bangalore 2"
    }
  ];
</script>

<style>

</style>

<Header />
<section id="meetups">
  {#each meetups as meetup}
    <MeetupItem
      title={meetup.title}
      subtitle={meetup.subtitle}
      description={meetup.description}
      imageUrl={meetup.imageUrl}
      address={meetup.address} />
  {/each}
</section>
