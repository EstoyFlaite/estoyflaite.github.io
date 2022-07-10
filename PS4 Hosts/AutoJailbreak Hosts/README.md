Bin2js instructions (To update GoldHen payload)

Put the .bin payload into "bin2js.exe", then edit the .js





At the beginning "var payload = [233,136,16..."

*Change "window.mira_blob_2_len = 251192;
window.mira_blob_2 = malloc(window.mira_blob_2_len);
write_mem(window.mira_blob_2, [233,136,16..."

to

"var payload = [233,136,16..." 





At the end "...55,101,102,54,53];"

*Delete the ")"

Ex:

After: "...55,101,102,54,53]);" (BAD)
Before: "...55,101,102,54,53];" (GOOD)