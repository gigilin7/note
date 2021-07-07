## 檢視電腦中可使用與目前所在的工作環境
`
conda env list
`

## 建立一個名稱為 test 的 Python 2 工作環境
`
conda create --name test python=2
`

## base->test
`
conda activate demo
`

## test->base
`
conda deactivate
`

## 查看python版本
`
python --version
`

## 檢視 test 工作環境中的套件
`
conda list --name test
`

## 移除 test 工作環境(要記得先執行conda deactivate回到base才能執行移除)
`
conda remove --name test --all
`

## 補充
+ Python 2 與 Python 3 程式語法有些不同，執行時要根據程式使用不同的工作環境
+ base通常是Python 3 工作環境
