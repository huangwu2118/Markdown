# Markdown作业

#### md链接：

 [README.md](README.md)

#### 图片链接：

![小姐姐](https://p.nanrenwo.net/uploads/allimg/180524/8472-1P524111347-52.jpg)
![谷歌](11.png)



这是一个链接 [baidu](https://www.baidu.com)



> 块引用
> > 111111
> >
> > > 222222





1. 第一项：
    - 1111111
    - 2222222
    
2. 第二项：
    - 3333333
    - 4444444
    
    
    
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
public:
    ListNode* addTwoNumbers(ListNode* l1, ListNode* l2) {
        ListNode *head = nullptr, *tail = nullptr;
        int carry = 0;
        while (l1 || l2) {
            int n1 = l1 ? l1->val: 0;
            int n2 = l2 ? l2->val: 0;
            int sum = n1 + n2 + carry;
            if (!head) {
                head = tail = new ListNode(sum % 10);
            } else {
                tail->next = new ListNode(sum % 10);
                tail = tail->next;
            }
            carry = sum / 10;
            if (l1) {
                l1 = l1->next;
            }
            if (l2) {
                l2 = l2->next;
            }
        }
        if (carry > 0) {
            tail->next = new ListNode(carry);
        }
        return head;
    }
};
~~~

