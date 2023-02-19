const books = [
    {
        name: "Javascript", price: "25.00"
    },
    {
        name: "PHP", price: "15.00"
    },
    {
        name: "Java", price: "30.00"
    },
    {
        name: "Elixir", price: "50.00"
    },
    {
        name: "GO", price: "45.00"
    },
    {
        name: "Python", price: "20.00"
    },
    {
        name: "Rust", price: "05.00"
    }
];

function GetLesserValueIndex(array, current) {
    let indexOfLesserValue = current;

    for (let i = current; i < array.length; i++) {
        if (Number(books[i].price) < Number(books[indexOfLesserValue].price)) {
            indexOfLesserValue = i;
        }
    }

    return indexOfLesserValue;
}

books.forEach((book, index) => {
    let lesserValue = GetLesserValueIndex(books, index);

    books[index] = books[lesserValue];
    books[lesserValue] = book;
})

console.log(books);