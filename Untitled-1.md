# <center>FirstMarkDown</center>
#一级标题
- 1.研究动物的控制器
- 2.研究动物的控制器
- 3.研究动物的控制器
- 4.研究动物的控制器
- 5.研究动物的控制器
- ---
## 二级标题
> 我的链接https:zanguapp.cn
---
### 三级标题
正常文字
*邪体文字*
**粗体文字**
~~删除线文字~~
'文字底纹'
`文字底纹`
  - [ ] 男   
  - [x] 女
---
#### 四级标题
[这是百度链接](https://www.baidu.com/)
![这是图片](Check.png)

---
##### 五级标题
|[姓名]|[密码]|班级|
|:----|:--:|--:|
|张三|123456789|六一班|
|李四|1231312|六二班|
---
###### 六级标题
```
void SetSelecedActor(int index)
{
    foreach (Transform trans in m_ModelParent)
        GameObject.Destroy(trans.gameObject);

    var id = m_ActorList[index];
    PlayerPrefs.SetInt("StoryModelActorID", id);
    Debug.Log("保存角色ID：" + PlayerPrefs.GetInt("StoryModelActorID"));
    var path = string.Format("ItemPrefabs/{0}/{1}/{2}", "Roles", id, id);
    var ob = Resources.Load<GameObject>(path);
    var go = GameObject.Instantiate(ob, m_ModelParent);
    go.transform.localScale = Vector3.one * 200.0f;
    go.transform.localEulerAngles = Vector3.up * 180.0f;
    go.transform.localPosition = new Vector3(0.0f, -250.0f, -150.0f);
    UIUtil.ChangeLayer(go.transform, "Animal");
}
```
---
[姓名]:该文章版权所有liangxing
[密码]:不可复制
