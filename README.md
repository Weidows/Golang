<!--
 * @?: *********************************************************************
 * @Author: Weidows
 * @Date: 2022-08-30 14:51:11
 * @LastEditors: Weidows
 * @LastEditTime: 2022-09-01 18:57:17
 * @FilePath: \Gmm\README.md
 * @Description:
 * @!: *********************************************************************
-->

> Some `demos` and `utils` in learning & developing golang.

<a>![分割线](https://www.helloimg.com/images/2022/07/01/ZM0SoX.png)</a>

# cmd

- <details>

    <summary> dsg | Disk sleep guard, 防止硬盘睡眠 </summary>

  ```shell
  go install github.com/Weidows/Golang/cmd/dsg@latest
  ```

  ***

  ```console
  > .\dsg.exe                                                                                                                                                                                                                                                               
  please start with params like: 'dsg.exe E: 30'
          1. disk
          2. delay seconds


  > dsg D:
  10 / 30 [------------------->_______________________________________] 33.33%
  ```

  </details>

- <details>

    <summary> gmm | Golang package Mirror Manager</summary>

  ```shell
  go install github.com/Weidows/Golang/cmd/gmm@latest
  ```

  ***

    ```console
    ╰─ gmm test
    proxys
            352ms   aliyun
            278ms   proxy-cn
            642ms   proxy-io
            269ms   baidu
            1002ms  tencent
            406ms   huawei
            837ms   default
    sumdbs
            2073ms  default
            789ms   google
            1957ms  sumdb-io
    ```

    ```console
    ╰─ gmm proxy huawei                                                                                                pwsh   95  12:17:56  
    Proxy use huawei https://repo.huaweicloud.com/repository/goproxy
    
    ╰─ gmm sumdb default                                                                                              pwsh   95  12:17:17 
    Sumdb use default https://sum.golang.org
    ```

  </details>

<a>![分割线](https://www.helloimg.com/images/2022/07/01/ZM0SoX.png)</a>

# utils

一些工具方法, 主要为了解决标准库中棘手/经常复用但没有的情况