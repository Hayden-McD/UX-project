<script>
    //Exports
    export let i;

    // Imports
    import { HISTORY } from "../assets/attendanceData";

    // Adding person history to array, then looping through the array to add seperators between each entry
    let historyArray = HISTORY[i].history;
    let finalData = "|";
    historyArray.forEach((element) => {
        finalData = finalData + " " + element + " |";
    });
</script>

<!-- Printing out the contents of the -->
<p class="history">
    {finalData}
</p>

<style>
    .history {
        display: flex;
        flex: 2;
        font-size: 18px;
        margin-right: 2rem;
    }
</style>
