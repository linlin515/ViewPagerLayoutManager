# ViewPager-LayoutManager [![Download](https://api.bintray.com/packages/rouchuan/maven/viewpager-layout-manager/images/download.svg) ](https://bintray.com/rouchuan/maven/viewpager-layout-manager/_latestVersion)

**English** | [中文](README_ZH.md)

VPLM is a `ViewPager` like `LayoutManager` which implements some common animations. If you need some other effects feel free to raise an issue or PR.

![circle](static/circle.gif) ![circle_scale](static/circle_scale.gif) ![carousel](static/carousel.gif) ![gallery](static/gallery.gif) ![rotate](static/rotate.gif) ![scale](static/scale.gif)

## Customzie

![customize](static/customize.gif)

Each layoutmanager has bunch of different properties to customize.

Such as:
* radius
* scroll speed
* space
* orientation

Run the demo to see more details.

## Infinite Scroll

![infinite](static/infinite.gif)

## Auto Center

![auto_center](static/auto_center.gif)

You can make the current position move to center automaticlly by:
```java
recyclerView.addOnScrollListener(new CenterScrollListener());
```

## Download

Gradle:

```groovy
repositories {
  jcenter()
}

dependencies {
  compile 'rouchuan.viewpagerlayoutmanager:viewpagerlayoutmanager:2.0.0'
}
```

Maven:

```xml
<dependency>
  <groupId>rouchuan.viewpagerlayoutmanager</groupId>
  <artifactId>viewpagerlayoutmanager</artifactId>
  <version>2.0.0</version>
  <type>pom</type>
</dependency>
```

## Quick Start
Make sure that each item has the same size, or something unpredictable may happen.

You can warm up your layoutmanager by builder.

```java
new CircleLayoutManager.Builder()
                .setAngleInterval(mAngle)
                .setMaxRemoveAngle(mMaxRemoveAngle)
                .setMinRemoveAngle(mMinRemoveAngle)
                .setMoveSpeed(mSpeed)
                .setRadius(mRadius)
                .setReverseLayout(true)
                .build();
```

Or just simply call the construct.

```java
new CircleLayoutManager();
```

## License

Apache-2.0. See [LICENSE](LICENSE) file for detail