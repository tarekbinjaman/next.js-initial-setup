# Follwoing this steps we can start a next.js project easily here we go

1. Run this:
~~~
npx create-next-app@latest my-frontend
~~~

2. It will ask questions → choose like this:
~~~
✔ TypeScript? → Yes
✔ ESLint? → Yes
✔ Tailwind CSS? → Yes
✔ App Router? → Yes (IMPORTANT)
✔ src/ directory? → Yes
✔ Import alias? → Yes
~~~

3. Then: 
~~~
cd my-frontend
~~~
Then enter  "code ." in cmd

Now, you will see your very first next.js files here

4. open:
npm run dev
[http://localhost:3000](http://localhost:3000)
5. Understand Next.js Structure (Very Important)
Inside src/app:

~~~
app/
 ├── layout.tsx   ← global layout
 ├── page.tsx     ← home page (/)
~~~

👉 In Next.js:
- page.tsx = route
- Folder name = URL

Example:

~~~
app/about/page.tsx → /about
~~~


5. Clean Setup (Recommended)

Delete everything inside page.tsx and write:

~~~
export default function Home() {
  return (
    <div>
      <h1>Hello Tarek 👋</h1>
    </div>
  );
}
~~~


6. Fix black backgroutnd

Go to:

~~~
src/app/globals.css
~~~

you probably see something like that:

~~~
:root {
  --background: #ffffff;
  --foreground: #000000;
}

@media (prefers-color-scheme: dark) {
  :root {
    --background: #0a0a0a;
    --foreground: #ededed;
  }
}

body {
  background: var(--background);
  color: var(--foreground);
}
~~~

replace with :

~~~
body {
  background: white;
  color: black;
}
~~~

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Till now you just installed your Next.js app but Real game start now!

From here you will start writing your component, functions, api and more.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------

# 🔥 Smart Developer Order (Remember This)

## 1. Layout + pages
## 2. Rgister
## 3. Login
## 4. Token store
## 5. Protected routes
## 6. Dashboard features