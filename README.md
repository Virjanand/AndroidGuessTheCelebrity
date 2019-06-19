# Guess the Celebrity
Android app in which a downloaded image (from http://www.posh24.se/kandisar) 
is displayed and the user has to guess the name of the celebrity out of four
randomly selected names from the same website.

# ToDo
- [x] Display one image in top half of screen
- [ ] Display 4 buttons in bottom half of screen
- [ ] Display name in button in bottom half of screen
- [ ] Display 3 random names in other buttons
- [ ] Suffle buttons
- [ ] When correct button is pressed display toast with correct
- [ ] When incorrect button is pressed: Wrong! It was ...

 String html= "<div class=\"image\"><img src=\"http://cdn.posh24.se/images/:profile/088110b3627723dd6f73b718905c2498f\" alt=\"Lady Gaga\"/></div>";
    
    Pattern p = Pattern.compile("src=\\\"(.*?)\"");
    Matcher m = p.matcher(html);
    
    while(m.find()) {
    	System.out.println(m.group(1));
    }
    
    p = Pattern.compile("alt=\\\"(.*?)\"");
    m = p.matcher(html);
    
    while(m.find()) {
    	System.out.println(m.group(1));
    }
  }