<script>
    // Exports
    export let person;

    // Formatting the date to YYYY-MM-DD
    let dob = person.dob.date;
    dob = dob.split("T")[0];
</script>

<div class="container">
    <img src={person.picture.large} alt="Student" class="profilePic" />
    <h2 class="name">{person.name.first} {person.name.last}</h2>
    <h3 class="dob">Date of birth: {dob}</h3>
    <h3 class="gender">Gender: {person.gender}</h3>
    <h3 class="phone">Phone: {person.cell}</h3>
    <h3 class="email">Email: {person.email}</h3>
    <h3 class="nat">Nationality: {person.nat}</h3>
</div>

<style>
    .container {
        display: flex;
        flex-direction: column;
    }

    .profilePic {
        margin: 0 auto;
    }

    h2 {
        display: flex;
        margin: 0 auto;
        margin-top: 1rem;
    }

    h3 {
        display: flex;
        margin: 0 auto;
        margin-top: 1rem;
    }
</style>
