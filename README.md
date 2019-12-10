[![](https://jitpack.io/v/milindrc/BackdropEasy.svg)](https://jitpack.io/#milindrc/BackdropEasy)

# BackdropEasy
A simple implementation of material design backdrop.


Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

Step 2. Add the dependency

	dependencies {
	        implementation 'com.github.milindrc:BackdropEasy:v0.1'
	}

# Usage

	public class TestActivity extends BackdropListActivity {

	    @Override
	    protected void onCreate(Bundle savedInstanceState) {
		super.onCreate(savedInstanceState);

	    }

	    @Override
	    public int getMenu() {
		return R.menu.main;
	    }

	    @Override
	    public Fragment getFragment(MenuItem item) {
		switch (item.getItemId()){
		    case R.id.a : return BlankFragment.newInstance("A","");
		    case R.id.b : return BlankFragment.newInstance("B", "");
		    case R.id.c: return BlankFragment.newInstance("C", "");
		    case R.id.d: return BlankFragment.newInstance("D", "");
		    case R.id.e: return BlankFragment.newInstance("E", "");
		    case R.id.f: return BlankFragment.newInstance("F", "");
		    case R.id.g: return BlankFragment.newInstance("G", "");
		    default: return null;
		}
	    }
	}
