# iOSCodeSnippets


## 使用方法
把文件导入Xcode目录 ==~/Library/Developer/Xcode/UserData/CodeSnippets==即可，
无则创建 CodeSnippets 目录。

## 规则


文件名 | 快捷键 | 代码段
----|------|----
mm-property-Assign| ppta |  @property (nonatomic, assign)
mm-property-Copy| pptcopy |  @property (nonatomic, copy)
mm-property-Strong| pptstrong |  @property (nonatomic, strong)
mm-property-Weak| pptweak |  @property (nonatomic, weak)
-||
mm-enum| men |  NS_ENUM
mm-opt| mopt |  NS_OPTIONS
mm-type-block| mtblock |  typedef block
-||
mm-rac_strongify| @s |  @strongify(self);
mm-rac_weakify| @w |  @weakify(self);
-||
mm-Log1| l1 |  NSLog(@"<#something#>");
mm-Log2| l2 |  NSLog(@"<#%#>", <#$#>);
mm-Mark| mark |  pragma mark
-||
mm-ObjectInit| minit |  init
mm-Shared| mshare |  单例
-||
mm-Picker| mpicker |  UIPickerView
mm-Table| mtab |  UITableView
mm-Collection| mcolle |  UICollectionView
-||
mm-Mantle| mtl |  MTLModel
mm-function-create| mfun |  create function


#### 同步共享工具
使用 [ACCodeSnippetRepositoryPlugin](https://github.com/acoomans/ACCodeSnippetRepositoryPlugin) 管理
> 目前不可用