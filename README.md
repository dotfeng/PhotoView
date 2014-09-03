PhotoView
=========

Implementation of ImageView for Android that supports zooming, by various touch gestures.

Sample with Android-Universal-Image-Loader https://github.com/nostra13/Android-Universal-Image-Loader


```Java
      PhotoView photoView = (PhotoView) findViewById(R.id.iv_photo);

        if (!ImageLoader.getInstance().isInited()) {
            ImageLoaderConfiguration config = new ImageLoaderConfiguration.Builder(getApplicationContext()).build();
            ImageLoader.getInstance().init(config);
        }

        ImageLoader.getInstance().displayImage("http://pbs.twimg.com/media/Bist9mvIYAAeAyQ.jpg", photoView);
```


```xml
    <uk.co.senab.photoview.PhotoView
      xmlns:android="http://schemas.android.com/apk/res/android"
      android:id="@+id/iv_photo"
      android:layout_width="fill_parent"
      android:layout_height="fill_parent"/>
```
