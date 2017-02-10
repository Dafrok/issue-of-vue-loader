# Guide

## Reproduction

Run these command and then visit [http://localhost:8080](http://localhost:8080).

```bash
git clone https://github.com/Dafrok/issue-of-vue-loader.git
cd issue-of-vue-loader
npm install
npm start
```

## Excepted Output

```html
<h2>GoodCase(Correctly mounted):</h2>
<div>A good case has been mounted here.</div>
<h2>## BadCase(can't be mounted and cause a warning):</h2>
<div>It's a bad case which will not be mounted.</div>
```

## Actual Output

```html
<h2>GoodCase(Correctly mounted):</h2>
<div>A good case has been mounted here.</div>
<h2>## BadCase(can't be mounted and cause a warning):</h2>
```

```
[Vue warn]: Invalid Component definition: ./BadCase.vue 
(found in anonymous component at fake-path/issue-of-vue-loader/src/App.vue)
```