<template>
  <!-- Display the upcoming activity directly from the google api -->
  <article class="message is-primary">
    <div class="message-body">
      <h1 class="title">
        {{ title }}
      </h1>
      <p>
        <strong>
          {{ date.toDateString() }}
        </strong>
      </p>
    </div>
  </article>
</template>

<script>
export default {
  data () {
    return {
      events: {},
      title: '',
      date: ''
    }
  },
  async mounted () {
    // Get the next event from google calendar api
    const datas = await fetch('https://www.googleapis.com/calendar/v3/calendars/gdf1s4irbjmjahl5llb69fs9i0@group.calendar.google.com/events?maxResults=1&key=AIzaSyBUXxBENyJmBErdt73ArFy9SUpOWvdaU2Y')
    this.events = await datas.json()
    this.title = this.events.items[0].summary
    this.date = new Date(this.events.items[0].start.dateTime)
  }
}
</script>
