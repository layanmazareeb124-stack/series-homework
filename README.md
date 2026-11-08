# SeriesHub Homework

This project is about TV series using JavaScript and JSON.

I created functions to find, sort, and update series without changing the original data.

## How to Run

To check the code:

`node check.js`

To save the updated data:

`node save-updated.js`

## Question 1

**Why is `{ ...show }` not enough in `addEpisode`?**

Because it only copies the show object, not the arrays inside it. I also need to copy the seasons and episodes so the original data does not change.

## Question 2

**Why did the spread operator not fix bug #3?**

Because `push()` changed the original episodes array before the copy was made. The spread operator only copied the show object, so the original data was still changed.