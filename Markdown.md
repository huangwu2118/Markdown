# Markdown作业

#### md链接：

 [README.md](README.md)

#### 图片链接：

![大数据](https://www.ruanyifeng.com/blogimg/asset/2017/bg2017122701.jpg)



这是一个链接 [baidu](https://www.baidu.com)



> 块引用
> > 第一层
> >
> > > 第二层





1. 第一项：
    - 第一个元素
    - 第二个元素
    
2. 第二项：
    - 第一个元素
    - 第二个元素
    
    
    
    |  1   |  2   |  3   |
    | :--: | :--: | :--: |
    |  4   |  5   |  6   |
    |  7   |  8   |  9   |
    
    **粗体文本**
    
    
    
    *斜体文本*
    
    ~~删除线~~
    
    *****
    
    
    
    

## 代码块：

~~~java
//两数之和
class Solution {
    public int[] twoSum(int[] nums, int target) {
        Map<Integer, Integer> hashtable = new HashMap<Integer, Integer>();
        for (int i = 0; i < nums.length; ++i) {
            if (hashtable.containsKey(target - nums[i])) {
                return new int[]{hashtable.get(target - nums[i]), i};
            }
            hashtable.put(nums[i], i);
        }
        return new int[0];
    }
}
~~~

