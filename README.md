solace
---

*a choc 1u sofle/alice-like keyboard*

built using [ergogen](https://ergogen.ceoloide.com/) & [flatfootfox's tutorial](https://flatfootfox.com/ergogen-introduction)

## links

- [ergogen](https://ergogen.ceoloide.com/)
- [ergogen docs](https://docs.ergogen.xyz/)
- [flatfootfox's tutorial](https://flatfootfox.com/ergogen-introduction)
- [ai03 Plate Generator](https://kbplate.ai03.com/)

## layout

![image](https://github.com/user-attachments/assets/0b288664-10b8-42ef-b2cd-85d69c58e383)

## build ergogen locally

to build the layout locally run:

```shell
npx ergogen layout.yaml
```

## build kle locally

```shell
# activate virtual environment
. .env/bin/activate.fish

# build kle from ergogen
python -m kbplacer.kle_serial -in output/points/points.yaml -inform ERGOGEN_INTERNAL -out solace-kle.json  -outform KLE_RAW

# leave virtualenv
deactivate
```

or

```shell
./.env/bin/python -m kbplacer.kle_serial -in output/points/points.yaml -inform ERGOGEN_INTERNAL -out solace-kle.json  -outform KLE_RAW
```