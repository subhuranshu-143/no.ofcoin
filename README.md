# no.ofcoin
Image procssing

ing=imread('coins.png");

imshow(ing)

Edge detection

in_boundary edge(ing);

imshow(im_boundary)

Filling gaps in the edges

filled_ing-infill(im_boundary, 'holes");

imshow(filled_ing)

Removing all noise

cleaned_ing-bwareaopen(filled_ing,100);

imshow(cleaned_ing)

Labelling and counting of coins

[L,num]=bwlabel(cleaned_ing);

imshow(L);

title(['Number of Coins:", num2str(num)]);

12

13

14

15

disp([Number of coins detected: num2str(num)]);

Coins in RGB

[L,num]-bwlabel(cleaned_ing);

imshow(label2rgb(L));

title(['Number of Coins:", num2str(num)]);

16

disp([Number of coins detected:num2str(num)]);
