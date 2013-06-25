class Library {

        array[] of Shelves;

        # constructor
        public Library(Shelves) {
                this->Shelves = Shelves;
        }

        function numberOfShelves() {
                return Shelves.count;
        }

        function numberOfBooks() {
                books = 0;
                foreach(books on Shelves) {
                        books += Shelves.numberOfBooks();
                }
                return books;
        }
}

class Shelf {

        array[] of Books;

        # constructor
        public Shelf(Books) {
                $this->Books = Books;
                foreach(Books) {
                        Book.setShelf(this);
                }
        }

        function numberOfBooks() {
                return Books.count();
        }

        function getBooks() {
                return Books;
        }
}

class Book {

        Shelf shelf;

        function setShelf(Shelf shelf) {
                shelf = shelf;
        }

        function enshelf {
                shelf.getBooks().putInArray(this);
        }

        function unshelf {
                shelf.getBooks().removeFromArray(this);
        }
}

main() {

        # create some books
        Book a = new Book();
        Book b = new Book();
        …
        # create some shelves
        Shelf shelf = new Shelf([a,b])
        ….
        # create a Library
        Library = new Library(shelves … )

        # number of books for library
        print(Library.numberOfShelves);

        # number of books for library
        print(Library.numberOfBooks);

        # enshelf
        a.enshelf;

        # unshelf
        b.unshelf;
}


