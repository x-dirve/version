# 版本比对

提供版本比较、范围匹配、匹配任意等功能

## 判断类型

- 比较版本 `compare`
    ```ts
    /**
    * 比较版本
    * @param  v1 样本版本
    * @param  v2 对比版本
    * @returns   对比结果：
    *              - 1 样本大于对比
    *              - 0 两者相等
    *              - -1 对比大于样本
    */
    function compare(v1: string, v2: string): 1 | -1 | 0;
    ```

- 匹配范围 `match`
    ```ts
    /**
    * 匹配范围
    * @param range 版本范围
    * @param v 对比版本
    */
    function match(range: string, v: string): boolean;
    ```

- 匹配任意
    ```ts
    /**
    * 匹配任意
    * @param range      范围
    * @param v          对比
    * @param ignoreCase 忽略大小写
    */
    function any(range: string, v: string, ignoreCase?: boolean): boolean;
    ```
