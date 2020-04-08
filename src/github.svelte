<script>
export let single;
import axios from 'axios';
let data = [];
let url = 'https://api.github.com/users';
if(!isNaN(single))
{
    url+="/"+single;
}
axios.get(url).then(e=>{
    data = data.concat(e.data);
});
</script>

<ul>
{#each data as d}
    <li>{d.login}- <br/>For data : {JSON.stringify(d)}</li>
{/each}

</ul>


<style>
</style>