<script>
	function createPost() {
		console.log('Created Post.');
	}
</script>

<!-- stylesheet for star ratings -->
<link
	rel="stylesheet"
	href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
/>

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

			<div class="acc">
				<img class="acc-img" src="/src/lib/img/avatar.jpg" alt="avatar" />
				<p class="acc-name">John Smith</p>
			</div>

			<div class="footer">
				<p class="footer_title">SMAP</p>
				<p class="footer_text">Placeholder</p>
			</div>
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
				<div class="sub-cards">
					<div class="placeholder" />
					<a href="/">Schedule</a>
				</div>
				<div class="sub-cards">
					<div class="placeholder" />
					<a href="/">Inventory</a>
				</div>
				<div class="sub-cards">
					<div class="placeholder" />
					<a href="/">Analytics</a>
				</div>
			</div>
			<div class="btm-sec">
				<!-- left=image right=placeholder -->
				<div>
					<img class="placeholder-img" src="/src/lib/img/placeholder.jpg" alt="placeholder" />
				</div>
				<div class="review-card">
					<p>Overall Review</p>
					<div class="rating">
						<div class="left-rating">
							<p class="num-rating">0.0</p>
							<div class="star-rating">
								<span class="fa fa-star" />
								<span class="fa fa-star" />
								<span class="fa fa-star" />
								<span class="fa fa-star" />
								<span class="fa fa-star" />
							</div>
						</div>
						<div class="meter-rating">
							<div>
								<p>5</p>
								<div class="meter" />
							</div>
							<div>
								<p>4</p>
								<div class="meter" />
							</div>
							<div>
								<p>3</p>
								<div class="meter" />
							</div>
							<div>
								<p>2</p>
								<div class="meter" />
							</div>
							<div>
								<p>1</p>
								<div class="meter" />
							</div>
						</div>
					</div>
					<div class="top-reviews">
						<p>Some dummy review texts here.</p>
					</div>
				</div>
			</div>
		</div>

		<div class="right-content">
			<div class="calendar">
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

			<div class="schedule">
				<p class="schedule-title">View Your Schedule</p>

				<div class="sub-schedule">placeholder</div>
				<div class="sub-schedule">placeholder</div>
				<div class="sub-schedule">placeholder</div>
			</div>
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
		width: 15%;
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

	.sideNav .acc {
		width: 100%;
		height: 15vh;
		position: absolute;
		bottom: 0;
	}

	.sideNav .acc .acc-img {
		height: auto;
		width: 15%;
		float: left;
	}

	.sideNav .acc .acc-name {
		color: black;
	}

	.sideNav .footer {
		width: 100%;
		height: 10vh;
		position: absolute;
		bottom: 0;
	}

	.sideNav .footer p {
		margin: 0;
		margin-top: 1vh;
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

	.middle-content a {
		text-decoration: none;
		display: block;
		transition: 0.2s;
		color: gray;
		border-radius: 12px;
		margin: 5px;
		padding: 10px;
	}

	.middle-content #searchBar input {
		width: 100%;
	}

	.middle-content .cards {
		display: flex;
		align-items: center;
		justify-content: center;
		margin: 10px;
	}

	.middle-content .cards .sub-cards {
		text-align: center;
		flex-direction: column;
	}

	.middle-content .cards .sub-cards .placeholder {
		width: 150px;
		height: 400px;
		background-color: pink;
		margin: 3%;
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		border-radius: 15px;
	}

	.middle-content .btm-sec .placeholder-img {
		transform: scale(50%);
		border: 5px solid black;
	}

	.middle-content .btm-sec .review-card {
		width: 20vw;
		height: auto;
		background-color: pink;
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		border-radius: 15px;
		flex-direction: column;
	}

	.middle-content .btm-sec .review-card p {
		color: red;
	}

	.middle-content .btm-sec .review-card .rating .left-rating {
		display: flex;
		flex-direction: column;
	}

	.middle-content .btm-sec .review-card .rating .left-rating .num-rating {
		color: white;
		font-size: large;
		margin: 0;
	}

	.middle-content .btm-sec .review-card .rating .left-rating .star-rating span {
		color: white;
	}

	.middle-content .btm-sec .review-card .rating .meter-rating {
		flex-direction: column;
	}

	.middle-content .btm-sec .review-card .rating .meter-rating div {
		margin: 0px;
		padding: 0px;
	}

	.middle-content .btm-sec .review-card .rating .meter-rating div p {
		margin-top: 0px;
		margin-bottom: 0px;
		margin-right: 2px;
		color: red;
	}

	.middle-content .btm-sec .review-card .rating .meter-rating div .meter {
		width: 100px;
		height: 4px;
		border: 2px solid red;
		border-radius: 15px;
		margin: 2px;
	}

	.middle-content .btm-sec .review-card .top-reviews {
		width: 90%;
		background-color: red;
		margin: 4px;
		border-radius: 15px;
	}

	.middle-content .btm-sec .review-card .top-reviews p {
		color: white;
	}

	.right-content .calendar {
		width: 125%;
		height: auto;
		box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
		float: right;
	}

	/* Month header */
	.right-content .calendar .month {
		padding: 70px 0px;
		width: 100%;
		background: red;
		text-align: center;
	}

	/* Month list */
	.right-content .calendar .month ul {
		margin: 0;
		padding: 0;
	}

	.right-content .calendar .month ul li {
		color: white;
		font-size: 20px;
		text-transform: uppercase;
		letter-spacing: 3px;
	}

	/* Previous button inside month header */
	.right-content .calendar .month .prev {
		float: left;
		list-style-type: none;
	}

	/* Next button */
	.right-content .calendar .month .next {
		float: right;
		list-style-type: none;
	}

	/* Weekdays (Mon-Sun) */
	.right-content .calendar .weekdays {
		margin: 0;
		padding: 10px 0;
		background-color: #ddd;
	}

	.right-content .calendar .weekdays li {
		display: inline-block;
		width: 13.6%;
		color: #666;
		text-align: center;
	}

	/* Days (1-31) */
	.right-content .calendar .days {
		padding: 10px 0;
		background: #eee;
		margin: 0;
	}

	.right-content .calendar .days li {
		list-style-type: none;
		display: inline-block;
		width: 13.6%;
		text-align: center;
		margin-bottom: 5px;
		font-size: 12px;
		color: #777;
	}

	.right-content .schedule {
		margin: 1vh;
	}

	.right-content .schedule .schedule-title {
		color: gray;
		text-align: center;
	}

	.right-content .schedule .sub-schedule {
		background-color: pink;
		color: white;
		width: 100%;
		height: 10vh;
		border-radius: 15px;
		margin: 0.5vh;
		text-align: center;
	}
</style>
