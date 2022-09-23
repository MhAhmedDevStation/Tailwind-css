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

#  Create  input.css in src
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
# To npm run dev 
##a compiler from input `html` to 
    `"dev":"tailwindcss -i ./src/input.css -o ./dist/output.css --watch"`,


# Or 
    `npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch`


input.css and output.css

    class="bg-black text-white"

