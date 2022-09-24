# Deal with tailwind CSS

Setup tailwind css through tailwind cli

## npm init

inisialise the project /node_module and package.json

## npm i -D tailwindcss

install tailwind

## npx tailwindcss init

create tailwind.config.js
to target html and js files

    content: ["./src/**/*.{html,js}"]

# Create input.css in src

    @tailwind base;
    @tailwind components;
    @tailwind utilities;

# To npm run dev

##a compiler from input `html` to
`"dev":"tailwindcss -i ./src/input.css -o ./dist/output.css --watch"`,

# Or

    `npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch`

input.css and output.css

# Classes

### background colors and text colors classes

    class="bg-black text-white"
            "bg-[brown]/50 text-[cyan]"

### Font sizing classes

    text-base // change font size =>
    text-xs
    text-md ,lg , xl ..
    < text-[25px]
    font-black
    capitalize
    uppercase
    ..

### Padding and margin classes

    pt-[20px]   only top
    pb          only bot
    pl          only left
    pr          only right
    px          left and right
    py          top and bot

    mx,my,mt,mb,ml,mr

## width and height Classes

@can use -mx-[value px] for minus value (negative)

    w-28
    w-2/12 take 2 columns from 12
    w-[50%]

    h-[10px]
    max-h-5

## borders and Radius Classes

    border-8            border-radius=8px
    rounded-full        koura
    border-dotted       mnaket
    rounded-br-full     90deg  bot-right
    rounded-tl-[30px]   top-left

## shadow classes

    shadow-2xl          taille
    shadow-orange-500"  give any color
    shadow-[skyblue]

    <div class=" bg-red-400 w-[300px] h-[300px] mx-auto mt-20 border-8 border-green-500 rounded-br-[30px] border-dashed shadow-2xl shadow-[skyblue]">

## gradient background

    bg-gradient-to-t    to-top
    bg-gradient-to-r    to-right
    from-green-400
    via-red-300
    to-green-900

## Before and After PseudoCLasses

    relative
    after:absolute
    after:top-full
    after:left-0
    after:w-full
    after:h-full
    after:bg-orange-600
    after:content-['Hello-world']

## Hover Effect

    bg-green-600
    text-white
    rounded
    hover:bg-rose-300
    transition-all
    duration-1000

## Flex box Flex Container

    <!-- flex in a row direction -->
     <div class="flex bg-red-500 flex-grow ">
        <div class="bg-gray-500 flex-grow-[2]">1</div>
        <div class="bg-red-500 flex-grow-[10]">2</div>
        <div class="bg-green-500 flex-grow">3</div>
        <div class="bg-blue-500 flex-grow">4</div>
    </div>

    flex-grow       take whoole availble space
    w-4/12          take 4 out of 12

    flex            1 2 3
    flex flex-wrap  1 2 3
                    4 5 6

## align items vertically and Horizantally
    justify-center/..           horizantally
    justify-evenly  between and arround equal spaces
    items-center/start/end/..   vertically

## basic difference between `block` elements and `inline` elmements

### `block` element
take the full width    

    <div></div>
    <section></section>
    <header></header>
    <p></p>
    <article></article>
    <footer></footer>

### `inline` element
    inline elements doesnt take the full width
    inline elements doesnt take the margin-top/bot 'my-20'

    block               transform inline element into block elemnt
    inline-block        |<buton>                                  |

    <a href=""></a>
    <span></span>
    <img src="" alt="">
    <ul></ul>
    <li></li>