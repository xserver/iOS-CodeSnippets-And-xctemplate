# iOS CodeSnippets And xctemplate
>代码规范，抓到放小，注意粒度，太细致则难以执行。
>通过 template and code snippets 可以解决一半问题

## UIViewController 模板

** 使用方法**
把`ViewController.xctemplate`
加入到
`/Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/Library/Xcode/Templates/File Templates/Source/`

``` Objective-C
@implementation Example


#pragma mark - Lifecycle
- (void)viewDidLoad {
    [super viewDidLoad];
    
}

- (void)dealloc {
    NSLog(@"%s %@", __FUNCTION__, NSStringFromClass([self class]));
}

#pragma mark - Views
- (void)addViews {
    
}


#pragma mark - Binding
- (void)binding {

}


#pragma mark - Methods


#pragma mark - Request


#pragma mark - Get Set Properties


#pragma mark - UITableView Delegate & DataSource


@end
```

## CodeSnippets
** 使用方法 **
把`CodeSnippets` 中的文件加入到Xcode目录
`~/Library/Developer/Xcode/UserData/CodeSnippets`，
无则创建 `CodeSnippets`。

## Shortcut Key
> 自己改快捷键，规定常用的即可。

文件名 | 快捷键 | 代码段
----|------|----
mm-property-Assign| pa |  @property (nonatomic, assign)
mm-property-Copy| pc |  @property (nonatomic, copy)
mm-property-Strong| ps |  @property (nonatomic, strong)
mm-property-Weak| pw |  @property (nonatomic, weak)
-||
mm-rac_strongify| @s |  @strongify(self);
mm-rac_weakify| @w |  @weakify(self);
-||
mm-Log1| l1 |  NSLog(@"");
mm-Log2| l2 |  NSLog(@"%@", );
-||
mm-Mark| mark |  #pragma mark - 
mm-ObjectInit| minit |  init
mm-Shared| mshare |  单例
-||
mm-enum| men |  NS_ENUM
mm-opt| mopt |  NS_OPTIONS
mm-type-block| mtb |  typedef block
-||
mm-Table| mtab |  UITableView
mm-Collection| mcolle |  UICollectionView
mm-Picker| mpicker |  UIPickerView



#### 同步共享工具
使用 [ACCodeSnippetRepositoryPlugin](https://github.com/acoomans/ACCodeSnippetRepositoryPlugin) 管理
> 目前不可用