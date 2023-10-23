<div class="sideNav">
    <button id="createPost" onclick="createPost()">Create Post</button>
    <div id="test"></div>
	<a href="/">Home &rsaquo;</a>
	<a href="/calendar">My Calendar &rsaquo;</a>
    <a href="/schedule">Schedule &rsaquo;</a>
    <a href="/inventory">Inventory &rsaquo;</a>
    <a href="/analytics">Analytics &rsaquo;</a>
    <a href="/invoices">Invoices &rsaquo;</a>
    <a href="/reviews">Post Reviews &rsaquo;</a>
    <a href="/contacts">Contacts &rsaquo;</a>
</div>

<style>
	.sideNav {
		height: 100%;
		position: fixed;
        border-right: solid gray 1px;
        padding-right: 10px;
	}

    .sideNav #createPost {
        background-color: red;
        color: white;
        font-size: 20px;
        border-radius: 12px;
        text-align: center;
        transition: 0.2s;
        border: 0px;
    }

    .sideNav #createPost:hover {
        background-color: pink;
    }

	.sideNav a {
		text-decoration: none;
        display: block;
        transition: 0.2s;
        color: gray;
        border-radius: 12px;
        margin: 5px;
	}

    .sideNav a:hover {
        color: red;
    }
</style>

<script>
    function createPost(){
        document.getElementById("test").innerHTML="test";
    }
</script>