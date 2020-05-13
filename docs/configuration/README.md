# Customization

## Customizing Fonts

Currently, there is no way to customize the fonts used by Melbourne. Support for changing the fonts used in the program has been added to the backlog of features to add, and should hopefully be available soon.

**Note**: While the `fonts/` folder is present in the resources folder, simply overriding these files with new fonts will not work as the font names are hard-coded in the application code. If these font files are deleted or renamed, the program *will* fail to start, so I highly recommend leaving them alone.

## Viewing Available Flags on Disk

To view the list of available flags to use in Melbourne, we can access the `flags/` resource folder to see the list of files.

* On Windows, the set of flags used by Melbourne can be found at `C:\Program Files (x86)\Melbourne\flags`.
* On macOS, accessing the `flags/` resource folder is slightly more involved but still easy. 
  - First, navigate to the `Applications/` folder where Melbourne is installed, right-click on the application and select `Show Package Contents`. Now, we can navigate to `Contents/Resources/flags` to view the set of available flags.

By default, there are three folders of flags: `ISC`, `World`, and `Rect`. To use flags from each of these folders, simply use the format `<folder>/<flag filename>` in the Excel spreadsheet (ex: `ISC/Kaledonii.png` or `World/ee.png`).

* **ISC** is the set of flags available for countries in the Internatia Song Contest on [escforum.net](http://escforum.net).
* **World** is a set of square flags available for real-world countries. Each country's flag is saved with its two letter ISO code in lowercase.
* **Rect** is a set of rectangular flags available for real-world countries. Similar to `World`, each country's flag is saved with its two letter ISO code in lowercase.
* Notes:
  - For both `World` and `Rect`, the flag for Serbia & Montenegro is available at `serbiamontenegro.png` — the country's ISO code was `yu` which would otherwise result in a naming conflict with the flag of Yugoslavia.
  - The flag of Kosovo is available at `xk.png`, following convention set by several international organizations such as the European Commission. Kosovo does not yet have an official ISO code as set by the International Organization for Standardization.

## Adding Custom Flags

To add custom flags, simply add additional flags to the `flags/` resource folder. 
* For example, if you wish to add a set of circular flags, create a `Circular` folder in the `flags` resource folder and add any flags inside that subfolder. To refer to any flag in this new folder, use `Circular/<flag filename>` in the input spreadsheet.

## List of Available Flags

Here, we can see the list of flags available in Melbourne, as of version `v5.1.0`.

### World Flags

In the table below, we can see the list of world flags available in the program. Not all of the square flags in the `World` folder have rectangular counterparts in the `Rect` folder.

| Flag | Country | World | Rect |
|:--------------------:|:------------------------------------------------:|:-----:|:----:|
| ad.png | Andorra | Yes | Yes |
| ae.png | United Arab Emirates | Yes | Yes |
| af.png | Afghanistan | Yes | Yes |
| ag.png | Antigua & Barbuda | Yes | Yes |
| ai.png | Anguilla (UK) | Yes | No |
| al.png | Albania | Yes | Yes |
| am.png | Armenia | Yes | Yes |
| ao.png | Angola | Yes | Yes |
| aq.png | Antarctica | Yes | No |
| ar.png | Argentina | Yes | Yes |
| as.png | American Samoa | Yes | No |
| at.png | Austria | Yes | Yes |
| au.png | Australia | Yes | Yes |
| aw.png | Aruba | Yes | No |
| ax.png | Åland Islands (Finland) | Yes | No |
| az.png | Azerbaijan | Yes | Yes |
| ba.png | Bosnia & Herzegovina | Yes | Yes |
| bb.png | Barbados | Yes | Yes |
| bd.png | Bangladesh | Yes | Yes |
| be.png | Belgium | Yes | Yes |
| bf.png | Burkina Faso | Yes | Yes |
| bg.png | Bulgaria | Yes | Yes |
| bh.png | Bahrain | Yes | Yes |
| bi.png | Burundi | Yes | Yes |
| bj.png | Benin | Yes | Yes |
| bl.png | Saint Barthélemy (France) | Yes | No |
| bm.png | Bermuda | Yes | No |
| bn.png | Brunei | Yes | Yes |
| bo.png | Bolivia | Yes | Yes |
| bq.png | Netherlands Antilles | Yes | No |
| br.png | Brazil | Yes | Yes |
| bs.png | The Bahamas | Yes | Yes |
| bt.png | Bhutan | Yes | Yes |
| bv.png | Bouvet Island (Norway) | Yes | No |
| bw.png | Botswana | Yes | Yes |
| by.png | Belarus | Yes | Yes |
| bz.png | Belize | Yes | Yes |
| ca.png | Canada | Yes | Yes |
| cc.png | Cocos Islands (Australia) | Yes | No |
| cd.png | Democratic Republic of the Congo | Yes | Yes |
| cf.png | Central African Republic | Yes | Yes |
| cg.png | Congo | Yes | Yes |
| ch.png | Switzerland | Yes | Yes |
| ci.png | Côte d'Ivoire (Ivory Coast) | Yes | Yes |
| ck.png | Cook Islands (New Zealand) | Yes | No |
| cl.png | Chile | Yes | Yes |
| cm.png | Cameroon | Yes | Yes |
| cn.png | China | Yes | Yes |
| co.png | Colombia | Yes | Yes |
| cr.png | Costa Rica | Yes | Yes |
| cu.png | Cuba | Yes | Yes |
| cv.png | Cabo Verde | Yes | Yes |
| cw.png | Curaçao (Netherlands) | Yes | No |
| cx.png | Christmas Island (Australia) | Yes | No |
| cy.png | Cyprus | Yes | Yes |
| cz.png | Czech Republic | Yes | Yes |
| de.png | Germany | Yes | Yes |
| dj.png | Djibouti | Yes | Yes |
| dk.png | Denmark | Yes | Yes |
| dm.png | Dominica | Yes | Yes |
| do.png | Dominican Republic | Yes | Yes |
| dz.png | Algeria | Yes | Yes |
| ec.png | Ecuador | Yes | Yes |
| ee.png | Estonia | Yes | Yes |
| eg.png | Egypt | Yes | Yes |
| eh.png | Western Sahara | Yes | Yes |
| er.png | Eritrea | Yes | Yes |
| es.png | Spain | Yes | Yes |
| et.png | Ethiopia | Yes | Yes |
| fi.png | Finland | Yes | Yes |
| fj.png | Fiji | Yes | Yes |
| fk.png | Falkland Islands (UK) | Yes | No |
| fm.png | Micronesia | Yes | Yes |
| fo.png | Faroe Islands (Denmark) | Yes | No |
| fr.png | France | Yes | Yes |
| ga.png | Gabon | Yes | Yes |
| gb.png | United Kingdom | Yes | Yes |
| gd.png | Grenada | Yes | Yes |
| ge.png | Georgia | Yes | Yes |
| gf.png | French Guiana | Yes | No |
| gg.png | Guernsey (UK) | Yes | No |
| gh.png | Ghana | Yes | Yes |
| gi.png | Gibraltar (UK) | Yes | No |
| gl.png | Greenland (Denmark) | Yes | No |
| gm.png | The Gambia | Yes | Yes |
| gn.png | Guinea | Yes | Yes |
| gp.png | Guadeloupe (France) | Yes | No |
| gq.png | Equatorial Guinea | Yes | Yes |
| gr.png | Greece | Yes | Yes |
| gs.png | South Georgia and the South Sandwch Islands (UK) | Yes | No |
| gt.png | Guatemala | Yes | Yes |
| gu.png | Guam (US) | Yes | No |
| gw.png | Guinea-Bissau | Yes | Yes |
| gy.png | Guyana | Yes | Yes |
| hk.png | Hong Kong | Yes | No |
| hm.png | Heard Island and McDonald Islands (Australia) | Yes | No |
| hn.png | Honduras | Yes | Yes |
| hr.png | Croatia | Yes | Yes |
| ht.png | Haiti | Yes | Yes |
| hu.png | Hungary | Yes | Yes |
| id.png | Indonesia | Yes | Yes |
| ie.png | Ireland | Yes | Yes |
| il.png | Israel | Yes | Yes |
| im.png | Isle of Man (UK) | Yes | No |
| in.png | India | Yes | Yes |
| io.png | British Indian Ocean Territory | Yes | No |
| iq.png | Iraq | Yes | Yes |
| ir.png | Iran | Yes | Yes |
| is.png | Iceland | Yes | Yes |
| it.png | Italy | Yes | Yes |
| je.png | Jersey (UK) | Yes | No |
| jm.png | Jamaica | Yes | Yes |
| jo.png | Jordan | Yes | Yes |
| jp.png | Japan | Yes | Yes |
| ke.png | Kenya | Yes | Yes |
| kg.png | Kyrgyzstan | Yes | Yes |
| kh.png | Cambodia | Yes | Yes |
| ki.png | Kiribati | Yes | Yes |
| km.png | Comoros | Yes | Yes |
| kn.png | St. Kitts & Nevis | Yes | Yes |
| kp.png | North Korea | Yes | Yes |
| kr.png | South Korea | Yes | Yes |
| kw.png | Kuwait | Yes | Yes |
| ky.png | Cayman Islands (UK) | Yes | No |
| kz.png | Kazakhstan | Yes | Yes |
| la.png | Laos | Yes | Yes |
| lb.png | Lebanon | Yes | Yes |
| lc.png | St. Lucia | Yes | Yes |
| li.png | Liechtenstein | Yes | Yes |
| lk.png | Sri Lanka | Yes | Yes |
| lr.png | Liberia | Yes | Yes |
| ls.png | Lesotho | Yes | Yes |
| lt.png | Lithuania | Yes | Yes |
| lu.png | Luxembourg | Yes | Yes |
| lv.png | Latvia | Yes | Yes |
| ly.png | Libya | Yes | Yes |
| ma.png | Morocco | Yes | Yes |
| mc.png | Monaco | Yes | Yes |
| md.png | Moldova | Yes | Yes |
| me.png | Montenegro | Yes | Yes |
| mf.png | Saint Martin (France) | Yes | No |
| mg.png | Madagascar | Yes | Yes |
| mh.png | Marshall Islands | Yes | Yes |
| mk.png | North Macedonia | Yes | Yes |
| ml.png | Mali | Yes | Yes |
| mm.png | Myanmar | Yes | Yes |
| mn.png | Mongolia | Yes | Yes |
| mo.png | Macau | Yes | No |
| mp.png | Northern Mariana Islands (US) | Yes | No |
| mq.png | Martinique (France) | Yes | No |
| mr.png | Mauritania | Yes | Yes |
| ms.png | Montserrat (UK) | Yes | No |
| mt.png | Malta | Yes | Yes |
| mu.png | Mauritius | Yes | Yes |
| mv.png | Maldives | Yes | Yes |
| mw.png | Malawi | Yes | Yes |
| mx.png | Mexico | Yes | Yes |
| my.png | Malaysia | Yes | Yes |
| mz.png | Mozambique | Yes | Yes |
| na.png | Namibia | Yes | Yes |
| nc.png | New Caledonia (France) | Yes | No |
| ne.png | Niger | Yes | Yes |
| nf.png | Norfolk Island (Australia) | Yes | No |
| ng.png | Nigeria | Yes | Yes |
| ni.png | Nicaragua | Yes | Yes |
| nl.png | Netherlands | Yes | Yes |
| no.png | Norway | Yes | Yes |
| np.png | Nepal | Yes | Yes |
| nr.png | Nauru | Yes | Yes |
| nu.png | Niue (New Zealand) | Yes | No |
| nz.png | New Zealand | Yes | Yes |
| om.png | Oman | Yes | Yes |
| pa.png | Panama | Yes | Yes |
| pe.png | Peru | Yes | Yes |
| pf.png | French Polynesia (France) | Yes | No |
| pg.png | Papua New Guinea | Yes | Yes |
| ph.png | The Philippines | Yes | Yes |
| pk.png | Pakistan | Yes | Yes |
| pl.png | Poland | Yes | Yes |
| pm.png | Saint Pierre and Miquelon (France) | Yes | No |
| pn.png | Pitcairn (UK) | Yes | No |
| pr.png | Puerto Rico | Yes | No |
| ps.png | Palestine | Yes | No |
| pt.png | Portugal | Yes | Yes |
| pw.png | Palau | Yes | Yes |
| py.png | Paraguay | Yes | Yes |
| qa.png | Qatar | Yes | Yes |
| re.png | Réunion (France) | Yes | No |
| ro.png | Romania | Yes | Yes |
| rs.png | Serbia | Yes | Yes |
| ru.png | Russia | Yes | Yes |
| rw.png | Rwanda | Yes | Yes |
| sa.png | Saudi Arabia | Yes | Yes |
| sb.png | Solomon Islands | Yes | Yes |
| sc.png | Seychelles | Yes | Yes |
| sd.png | Sudan | Yes | Yes |
| se.png | Sweden | Yes | Yes |
| serbiamontenegro.png | Serbia & Montenegro | Yes | Yes |
| sg.png | Singapore | Yes | Yes |
| sh.png | St. Helena | Yes | No |
| si.png | Slovenia | Yes | Yes |
| sj.png | Svalbard and Jan Mayen (Norway) | Yes | No |
| sk.png | Slovakia | Yes | Yes |
| sl.png | Sierra Leone | Yes | Yes |
| sm.png | San Marino | Yes | Yes |
| sn.png | Senegal | Yes | Yes |
| so.png | Somalia | Yes | Yes |
| sr.png | Suriname | Yes | Yes |
| ss.png | South Sudan | Yes | No |
| st.png | São Tomé and Príncipe | Yes | Yes |
| sv.png | El Salvador | Yes | Yes |
| sx.png | Sint Maarten (Netherlands) | Yes | No |
| sy.png | Syria | Yes | Yes |
| sz.png | eSwatini | Yes | Yes |
| tc.png | Turks and Caicos (UK) | Yes | No |
| td.png | Chad | Yes | Yes |
| tf.png | French Southern Territories | Yes | No |
| tg.png | Togo | Yes | Yes |
| th.png | Thailand | Yes | Yes |
| tj.png | Tajikistan | Yes | Yes |
| tk.png | Tokelau (New Zealand) | Yes | No |
| tl.png | Timor Leste | Yes | Yes |
| tm.png | Turkmenistan | Yes | Yes |
| tn.png | Tunisia | Yes | Yes |
| to.png | Tonga | Yes | Yes |
| tr.png | Turkey | Yes | Yes |
| tt.png | Trinidad & Tobago | Yes | Yes |
| tv.png | Tuvalu | Yes | Yes |
| tw.png | Taiwan | Yes | Yes |
| tz.png | Tanzania | Yes | Yes |
| ua.png | Ukraine | Yes | Yes |
| ug.png | Uganda | Yes | Yes |
| uk.png | United Kingdom | Yes | No |
| um.png | Northern Mariana Islands (US) | Yes | No |
| us.png | United States | Yes | Yes |
| uy.png | Uruguay | Yes | Yes |
| uz.png | Uzbekistan | Yes | Yes |
| va.png | Vatican City | Yes | Yes |
| vc.png | Saint Vincent and the Grenadines | Yes | Yes |
| ve.png | Venezuela | Yes | Yes |
| vg.png | British Virgin Islands | Yes | No |
| vi.png | US Virgin Islands | Yes | No |
| vn.png | Vietnam | Yes | Yes |
| vu.png | Vanuatu | Yes | Yes |
| wf.png | Wallis and Futuna (France) | Yes | No |
| ws.png | Samoa | Yes | Yes |
| xk.png | Kosovo | Yes | Yes |
| ye.png | Yemen | Yes | Yes |
| yt.png | Mayotte (France) | Yes | No |
| yu.png | Yugoslavia | Yes | Yes |
| za.png | South Africa | Yes | Yes |
| zm.png | Zambia | Yes | Yes |
| zw.png | Zimbabwe | Yes | Yes |

### ISC/OSC Flags

| Flag | Country |
|:------------------------------:|:-----------------------------------:|
| Aevis.png | Aevis |
| Ahraspen.jpg | Ahraspen |
| Alardon.png | Alardon |
| Alexandria.jpg | Alexandria |
| Alma Livre.png | Alma Livre |
| Almarania.png | Almarania |
| Alteus.png | Alteus |
| Amika.png | Amika |
| Amsteris.png | Amsteris |
| Angellandia.png | Angellandia |
| Anselmsuusonia.png | Anselmsuusonia |
| Aonach.png | Aonach |
| Arcorar.png | Arcorar |
| Asankon.png | Asankon |
| Atsoumpalia.png | Atsoumpalia |
| Auravaan.png | Auravään |
| Auspikitan.png | Auspikitan |
| Bartlett.png | Bartlett |
| Beige.png | Beige |
| Bitland.png | Bitland |
| Brickistan.png | Brickistan |
| Bubblique.png | Bubblique |
| Canedonia.png | Canedonia |
| Caprika.png | Caprika |
| Carpathia.png | Carpathia |
| Celestiana.png | Celestiana |
| Chimeria.png | Chimeria |
| Chruno.png | Chruno |
| Cytrus.png | Cytrus |
| Dagon-Azuria.png | Dagon-Azuria |
| Darkria.png | Darkria |
| Daulska.png | Daǔlska |
| DimkaRUS.png | DimkaRUS |
| Dinokratys & Shrikidai.png | Dinokratys & Shrikidai |
| DPR Jindalea.png | DPR Jindalea |
| Dulcet Ebullience.png | Dulcet Ebullience |
| Dvipantara.png | Dvipantara |
| Easterosia.png | Easterosia |
| Edoriada.png | Edoriada |
| EdvinOla.jpg | EdvinOla |
| Ekotruka.png | Ekotruka |
| Enot'ebia.png | Enot'ebia |
| Eriod.png | Eriod |
| Evergreen Lands.png | Evergreen Lands |
| Falvarak.png | Faĺvarak |
| Fervorosia.jpg | Fervorosia |
| Fierce.png | Fierce |
| Folkloria.png | Folkloria |
| Frostfall.png | Frostfall |
| Gandhara.png | Gandhara |
| Gebze.png | Gebze |
| Grolskira.png | Grolskira |
| Hanei Caravaz.png | Ħanei Čaravāz |
| Hanzyuki.png | Hanzyuki |
| Harlequenia.png | Harlequenia |
| Hattuka.png | Hattuka |
| Haven.png | Háttųka |
| HKJIADH.png | H Kim Jong Il's AD Hangug (HKJIADH) |
| Huania.png | Huania |
| Irdminia.png | Irdminia |
| Irlandia.png | Irlandia |
| Ivanotia.png | Ivanotia |
| Jhe Freeh.png | Jhe Freeh |
| Jungalero.png | Jungalero |
| Kaeros Islands.png | Kaeros Islands |
| Kaledonii.png | Kaledonii |
| Kaministiquia.png | Kaministiquia |
| Kannel.png | Kannel |
| Karuex and Qargering.png | Karuex and Qargering |
| Keohretcha.png | Keohretcha |
| Kharo.jpg | Kharó |
| Kilvan League.png | Kilvan League |
| Kimmystan.png | Kimmystan |
| Koalatopolous.png | Koalatopolous |
| Kosma.png | Kosma |
| Kox-Zoeteweij.png | Kox-Zoeteweij |
| Kwonia.png | Kwonia |
| Lacrea.png | Lacrea |
| Ladoga.png | Ladoga |
| Lahna.png | Lahna |
| Laranjeirian Confederation.png | Laranjeirian Confederation |
| Leshia.png | Leshia |
| Lettuce.png | Lettuce |
| Levie.png | Levie |
| Limnoupolitana.png | Limnoupolitana |
| LM Lazovi.png | L.M. Lažovi |
| Lost Islands.png | Lost Islands |
| Luzze.png | Luzze |
| Marium.png | Mărium |
| Marvelia.png | Marvelia |
| Mensa.png | Men̈́sa |
| Monteverde.png | Monteverde |
| Multakin.png | Multakin |
| Nickymania.png | Nickymania |
| Nicolas' Neighbour.png | Nicolas' Neighbour |
| Nouvelle-Acadie.png | Nouvelle-Acadie |
| Novatlantida.png | Novatlantida |
| Noxus.png | Noxus |
| Oalia.png | Oalia |
| Oravania.jpg | Oravania |
| Ova Anova.png | Ova Anova |
| Pebbleland.png | Pebbleland |
| Pen Island.png | Pen Island |
| Percheron.png | Percheron |
| Pinnipedia.png | Pinnipedia |
| Polland.png | Polland |
| Ponasikwa.png | Ponásikwa |
| Pono.png | Pönö |
| Porielana.png | Porielana |
| Puntikov.png | Puntíkov |
| Radamede.png | Radamede |
| Raingate.png | Raingate |
| Randomia.png | Randomia |
| Rata Sum.png | Rata Sum |
| RC Laranjeiras.png | RC Laranjeiras |
| Republica Libera.png | Republica Libera |
| Riya-Sampetrina.png | Riya-Sampetrina |
| Rotenrod.png | Rötenrod |
| Ruthsina.png | Ruthsina |
| San Monique.png | San Monique |
| San Remo.png | San Remo |
| Sanlyona.png | Sanlyona |
| Saonas Fe Pier.jpg | Saónas Fe Pier |
| Satoriland.png | Satoriland |
| SEAL.png | St. Eva & Lepland |
| Sibinia.png | Sibinia |
| Sockistan.png | Sockistan |
| Solais X.png | Solais X |
| Spinachia.png | Spinachia |
| Spirevo.png | Spirevo |
| Spitzenbergen.png | Spitzenbergen |
| St Laurentis.png | St Laurentis |
| St Olaf.png | St Olaf |
| St. Eva & Lepland.png | St. Eva & Lepland |
| St. Olaf.png | St. Olaf |
| Style.jpg | Stylé |
| Sunetti.png | Sunetti |
| Swelatie.png | Swelatie |
| Symphony Isles.png | Symphony Isles |
| Tashkveny.png | Tashkveny |
| Territrius.png | Territrius |
| TETRIS.png | TETRIS |
| Thorway.png | Thorway |
| Tikata.png | Tikata |
| Timivar.png | Timivar |
| Tjarsklanjska.png | Tjärsklanjska |
| Tonallan.png | Tonallán |
| Treslend.png | Trešland |
| Trolofloppia.png | Trolofloppia |
| Unovah.png | Unovah |
| Uubell.png | Uubell |
| Uurnikoise.png | Üürnikoise |
| V.png | V |
| Valdron.png | Valdron |
| Victoria.png | Victoria |
| Volnytaria.png | Volnytaria |
| Waticania.png | Waticania |
| West Bombo.png | West Bombo |
| Winterlune.png | Winterlune |
| Xara Khanate.png | Xara Khanate |
| Xhanostania.png | Xhanostania |
| Yazminia.png | Yazminia |
| Yutuland.png | Yutuland |
| Zelmerlowia.png | Zelmerlowia |
| Zeme Kuku.png | Zeme Kūku |
| Zephyrus.png | Zephyrus |