cars
======
@@ p final String getInfo(String s) {
150	150	 
151	151	         String info;
152	152	 
153		-        if (!new File(s).exists())
153	+        if (s == null || (!new File(s).exists()))
154	154	             return "Unavailable";
155	155	 
156	156	         try {
