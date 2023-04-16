# next.js

## example

```shell
$ npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn/tree/master/basics/learn-starter"
$ cd nextjs-blog
$ npm run dev
$ yarn dev
# http://localhost:3000/
```

- vercel commerce sample

```shell
$ git clone https://github.com/vercel/commerce.git
```

## start next.js

### Fetching

- SSR: Server Side Render
  - getServerSideProps()
- CSR: Client Side Render
  - nothing to do
- SSG: Static Side Generation
  - 정적인 사이트 생성 (데이터를 가져와서 그려둔다.)
  - build 해야 적용, 빌드하지 않으면 SSR로 동작 (yarn build; yarn start)
  - getStaticProps
  - (with) getStaticPaths
- ISR: Incremental Static Regeneration
  - 증분 정적 사이트를 재생성한다
  - (특정 주기로) 정적인 사이트를 데이터를 가져와서 다시 그려둔다.
  - getSataticProps with revalidate
  - SSG 장점 + SSR 장점
