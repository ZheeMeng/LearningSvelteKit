<script>
	function createPost() {
		console.log('Created Post.');
	}
</script>

<body>
	<div class="content">
		<div class="sideNav">
			<!-- update createPost function -->
			<button id="createPost" on:click={createPost}>Create Post</button>
			<a href="/">Home &rsaquo;</a>
			<a href="/calendar">My Calendar &rsaquo;</a>
			<a href="/schedule">Schedule &rsaquo;</a>
			<a href="/inventory">Inventory &rsaquo;</a>
			<a href="/analytics">Analytics &rsaquo;</a>
			<a href="/invoices">Invoices &rsaquo;</a>
			<a href="/reviews">Post Reviews &rsaquo;</a>
			<a href="/contacts">Contacts &rsaquo;</a>
		</div>

		<div class="middle-content">
			<div id="searchBar">
				<input type="text" placeholder="search somthing" />
				<button type="submit">Search</button>
			</div>
			<div id="titles">
				<!-- add in href -->
				<a href="/">Quick Access</a>
				<a href="/">What's New</a>
				<a href="/">Updates</a>
			</div>
			<div class="cards">
				<!-- add in href -->

				<!-- !!!card & text alignment to be completed!!! -->
				<div class="sub-cards">
					<div class="placeholder"></div>
					<a href="/">Schedule</a>
				</div>
				<div class="sub-cards">
					<div class="placeholder"></div>
					<a href="/">Inventory</a>
				</div>
				<div class="sub-cards">
					<div class="placeholder"></div>
					<a href="/">Analytics</a>
				</div>
			</div>
		</div>

		<div class="right-content">
			<div class="month">
				<ul>
					<li class="prev">&lsaquo;</li>
					<li class="next">&rsaquo;</li>
					<li>August<br /><span style="font-size:18px">2023</span></li>
				</ul>
			</div>

			<ul class="weekdays">
				<li>Mo</li>
				<li>Tu</li>
				<li>We</li>
				<li>Th</li>
				<li>Fr</li>
				<li>Sa</li>
				<li>Su</li>
			</ul>

			<ul class="days">
				<li>1</li>
				<li>2</li>
				<li>3</li>
				<li>4</li>
				<li>5</li>
				<li>6</li>
				<li>7</li>
				<li>8</li>
				<li>9</li>
				<li>10</li>
				<li>11</li>
				<li>12</li>
				<li>13</li>
				<li>14</li>
				<li>15</li>
				<li>16</li>
				<li>17</li>
				<li>18</li>
				<li>19</li>
				<li>20</li>
				<li>21</li>
				<li>22</li>
				<li>23</li>
				<li>24</li>
				<li>25</li>
				<li>26</li>
				<li>27</li>
				<li>28</li>
				<li>29</li>
				<li>30</li>
				<li>31</li>
			</ul>
		</div>
	</div>
</body>

<style>
	.content {
		display: flex;
	}

	.sideNav {
		float: left;
		width: 25%;
		height: 100%;
		position: fixed;
		/* border-right: solid gray 1px; */
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

	.middle-content {
		float: left;
		width: 50%;
		margin: 0 auto;
	}

	.middle-content div {
		display: flex;
		align-items: center;
		justify-content: center;
		margin: 10px;
	}

	.middle-content .cards {
		display: flex;
		align-items: center;
		justify-content: center;
		margin: 10px;
	}

	.middle-content .cards .sub-cards {
		text-align: center;
	}

	.middle-content .cards .sub-cards .placeholder {
		width: 30%;
		height: 400px;
		background-color: gray;
		margin: 3%;
	}

	.middle-content a {
		text-decoration: none;
		display: block;
		transition: 0.2s;
		color: gray;
		border-radius: 12px;
		margin: 5px;
		padding: 10px;
	}

	.right-content {
		width: 25%;
		float: right;
	}

	/* Month header */
	.right-content .month {
		padding: 70px 0px;
		width: 100%;
		background: red;
		text-align: center;
	}

	/* Month list */
	.right-content .month ul {
		margin: 0;
		padding: 0;
	}

	.right-content .month ul li {
		color: white;
		font-size: 20px;
		text-transform: uppercase;
		letter-spacing: 3px;
	}

	/* Previous button inside month header */
	.right-content .month .prev {
		float: left;
		list-style-type: none;
	}

	/* Next button */
	.right-content .month .next {
		float: right;
		list-style-type: none;
	}

	/* Weekdays (Mon-Sun) */
	.right-content .weekdays {
		margin: 0;
		padding: 10px 0;
		background-color: #ddd;
	}

	.right-content .weekdays li {
		display: inline-block;
		width: 13.6%;
		color: #666;
		text-align: center;
	}

	/* Days (1-31) */
	.right-content .days {
		padding: 10px 0;
		background: #eee;
		margin: 0;
	}

	.right-content .days li {
		list-style-type: none;
		display: inline-block;
		width: 13.6%;
		text-align: center;
		margin-bottom: 5px;
		font-size: 12px;
		color: #777;
	}
</style>
