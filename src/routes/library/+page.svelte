<svelte:head>
	<title>Infinity Archives | Library</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">
	<h1>Library</h1>

	<p>
		Welcome to the library of the Infinity Archives. You can search the library by just searching
		anything in the search bar, yet I would recommend you to turn on the filters to narrow down your
		search.
	</p>

	<p>
		So in case you want to search by year, you can just click on the year filter and then type in
		the year you want to search for... You can also search by multiple filters at once, so if you
        want to search for a book that was published in 2010 and is a fantasy book, you can just activate
        both filters and then type in the year and the genre.
	</p>

    <br>

	<div class="filters">
		<div class="column">
			<button class="filter">Genre</button>
		</div>

		<div class="column">
			<button class="filter">Cover colors</button>
		</div>

		<div class="column">
			<button class="filter">Author</button>
		</div>

		<div class="column">
			<button class="filter">Year</button>
		</div>

		<div class="column">
			<button class="filter">Language</button>
		</div>

		<div class="column">
			<button class="filter">Publisher</button>
		</div>

		<div class="column">
			<button class="filter">ISBN</button>
		</div>

		<div class="column">
			<button class="filter">Our rating 1-5</button>
		</div>
	</div>

	<div class="column">
		<input type="search" placeholder="Just search already bro..." />
	</div>
</div>

<style>
	input {
		width: 100%;
		padding: 0.5rem;
        border: 1px solid black;
		border-radius: 4px;
		margin-bottom: 1rem;
        transition: all 0.3s ease-in-out;
	}

    input:focus {
        box-shadow: 0 0 30px rgba(0, 0, 0, 0.244);
    }

	.filters {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-between;
		margin-bottom: 1rem;
	}

    .filter {
        padding: 0.4rem .8rem;
        border: 1px solid black;
        background-color: white;
        border-radius: 4px;
        color: var(--text);
        margin-bottom: 0.5rem;
        transition: all 0.3s ease-in-out;
    }

    .filter:hover {
        box-shadow: 0 0 30px rgba(0, 0, 0, 0.244);
        color: white;
        background-color: black;
        cursor: pointer;
    }

    .column {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
