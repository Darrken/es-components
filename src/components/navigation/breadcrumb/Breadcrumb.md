Use breadcrumbs to chain a list of items together
```
function Link({destination, name}){
  return <a href={`#${destination}`} style={{textDecorationLine: 'none'}}>{name}</a>
}

function Location({name}){
  return <span>{name}</span>
}

   <Breadcrumb className="test" name="nav">
    <Link name="home" destination="bye there"/>
    <Button name="gettingThere" handleOnClick={() => alert("on my way")} styleType="accent">getting there</Button>
    <Link name="test" destination="bye"/>
    <Location name="destination"/>
  </Breadcrumb>

```