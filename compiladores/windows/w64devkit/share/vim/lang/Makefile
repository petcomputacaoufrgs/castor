# Author: Ada (Haowen) Yu <me@yuhaowen.com>

all: \
		menu_chinese_gb.936.vim \
		menu_uk_ua.cp1251.vim \
		menu_uk_ua.koi8-u.vim \
		menu_chinese_taiwan.950.vim \
		menu_cs_cz.iso_8859-2.vim \
		menu_czech_czech_republic.1250.vim \
		menu_ja_jp.euc-jp.vim \
		menu_japanese_japan.932.vim \
		menu_ko_kr.euckr.vim \
		menu_pl_pl.iso_8859-2.vim \
		menu_polish_poland.1250.vim \
		menu_ru_ru.koi8-r.vim \
		menu_sl_si.cp1250.vim \
		menu_sl_si.latin2.vim \
		menu_slovak_slovak_republic.1250.vim \
		menu_tr_tr.cp1254.vim \
		menu_tr_tr.iso_8859-9.vim \
		menu_sr_rs.iso_8859-5.vim \
		menu_sr_rs.iso_8859-2.vim \
		menu_sr_rs.ascii.vim \
		menu_czech_czech_republic.ascii.vim \

# Convert menu_zh_cn.utf-8.vim to create menu_chinese_gb.936.vim.
menu_chinese_gb.936.vim: menu_zh_cn.utf-8.vim
	rm -f menu_chinese_gb.936.vim
	iconv -f utf-8 -t cp936 menu_zh_cn.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp936/' -e 's/" Original translations/" Generated from menu_zh_cn.utf-8.vim, DO NOT EDIT/' > menu_chinese_gb.936.vim

# Convert menu_zh_tw.utf-8.vim to create menu_chinese_taiwan.950.vim.
menu_chinese_taiwan.950.vim: menu_zh_tw.utf-8.vim
	rm -f menu_chinese_taiwan.950.vim
	iconv -f utf-8 -t cp950 menu_zh_tw.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp950/' -e 's/" Original translations/" Generated from menu_zh_tw.utf-8.vim, DO NOT EDIT/' > menu_chinese_taiwan.950.vim

# Convert menu_cs_cz.utf-8.vim to create menu_cs_cz.iso_8859-2.vim.
menu_cs_cz.iso_8859-2.vim: menu_cs_cz.utf-8.vim
	rm -f menu_cs_cz.iso_8859-2.vim
	iconv -f utf-8 -t iso8859-2 menu_cs_cz.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding iso8859-2/' \
			-e 's/" Original translations/" Generated from menu_cs_cz.utf-8.vim, DO NOT EDIT/' \
			-e 's/\(" Menu Translations:.*\)(.*)/\1(ISO8859-2)/'  \
			> menu_cs_cz.iso_8859-2.vim

# Convert menu_cs_cz.utf-8.vim to create menu_czech_czech_republic.1250.vim.
menu_czech_czech_republic.1250.vim: menu_cs_cz.utf-8.vim
	rm -f menu_czech_czech_republic.1250.vim
	iconv -f utf-8 -t cp1250 menu_cs_cz.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp1250/'  \
		-e 's/" Original translations/" Generated from menu_cs_cz.utf-8.vim, DO NOT EDIT/'  \
		-e 's/\(" Menu Translations:.*\)(.*)/\1(CP1250)/'  \
		> menu_czech_czech_republic.1250.vim

# Convert menu_cs_cz.utf-8.vim to create menu_czech_czech_republic.ascii.vim.
menu_czech_czech_republic.ascii.vim: menu_cs_cz.utf-8.vim
	rm -f menu_czech_czech_republic.ascii.vim
	sed -e 's/??/A/g' -e 's/??/a/g' -e 's/??/C/g' -e 's/??/c/g' -e 's/??/D/g' \
		-e 's/??/d/g' -e 's/??/E/g' -e 's/??/e/g' -e 's/??/E/g' -e 's/??/e/g' \
		-e 's/??/I/g' -e 's/??/i/g' -e 's/??/N/g' -e 's/??/n/g' -e 's/??/O/g' \
		-e 's/??/o/g' -e 's/??/R/g' -e 's/??/r/g' -e 's/??/S/g' -e 's/??/s/g' \
		-e 's/??/T/g' -e 's/??/t/g' -e 's/??/U/g' -e 's/??/u/g' -e 's/??/U/g' \
		-e 's/??/u/g' -e 's/??/Y/g' -e 's/??/y/g' -e 's/??/Z/g' -e 's/??/z/g' \
		-e 's/scriptencoding utf-8/scriptencoding latin1/'  \
		-e 's/" Original translations/" Generated from menu_cs_cz.utf-8.vim, DO NOT EDIT/' \
		-e 's/\(" Menu Translations:.*\)(.*)/\1(ASCII - without diacritics)/'  \
	menu_cs_cz.utf-8.vim > menu_czech_czech_republic.ascii.vim

# Convert menu_ja_jp.utf-8.vim to create menu_ja_jp.euc-jp.vim.
menu_ja_jp.euc-jp.vim: menu_ja_jp.utf-8.vim
	rm -f menu_ja_jp.euc-jp.vim
	iconv -f utf-8 -t euc-jp menu_ja_jp.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding euc-jp/'  \
		-e 's/" Original translations/" Generated from menu_ja_jp.utf-8.vim, DO NOT EDIT/'  \
		-e 's/\(" Menu Translations:.*\)(.*)/\1(EUC-JP)/'  \
		> menu_ja_jp.euc-jp.vim

# Convert menu_ja_jp.utf-8.vim to create menu_japanese_japan.932.vim.
menu_japanese_japan.932.vim: menu_ja_jp.utf-8.vim
	rm -f menu_japanese_japan.932.vim
	iconv -f utf-8 -t cp932 menu_ja_jp.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp932/'  \
		-e 's/" Original translations/" Generated from menu_ja_jp.utf-8.vim, DO NOT EDIT/' \
		-e 's/\(" Menu Translations:.*\)(.*)/\1(CP932)/'  \
		> menu_japanese_japan.932.vim

# Convert menu_ko_kr.utf-8.vim to create menu_ko_kr.euckr.vim.
menu_ko_kr.euckr.vim: menu_ko_kr.utf-8.vim
	rm -f menu_ko_kr.euckr.vim
	iconv -f utf-8 -t euc-kr menu_ko_kr.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding euc-kr/' -e 's/" Original translations/" Generated from menu_ko_kr.utf-8.vim, DO NOT EDIT/' > menu_ko_kr.euckr.vim

# Convert menu_pl_pl.utf-8.vim to create menu_pl_pl.iso_8859-2.vim.
menu_pl_pl.iso_8859-2.vim: menu_pl_pl.utf-8.vim
	rm -f menu_pl_pl.iso_8859-2.vim
	iconv -f utf-8 -t iso8859-2 menu_pl_pl.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding iso8859-2/' -e 's/" Original translations/" Generated from menu_pl_pl.utf-8.vim, DO NOT EDIT/' > menu_pl_pl.iso_8859-2.vim

# Convert menu_pl_pl.utf-8.vim to create menu_polish_poland.1250.vim.
menu_polish_poland.1250.vim: menu_pl_pl.utf-8.vim
	rm -f menu_polish_poland.1250.vim
	iconv -f utf-8 -t cp1250 menu_pl_pl.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp1250/' -e 's/" Original translations/" Generated from menu_pl_pl.utf-8.vim, DO NOT EDIT/' > menu_polish_poland.1250.vim

# Convert menu_ru_ru.utf-8.vim to create menu_ru_ru.koi8-r.vim.
menu_ru_ru.koi8-r.vim: menu_ru_ru.utf-8.vim
	rm -f menu_ru_ru.koi8-r.vim
	iconv -f utf-8 -t koi8-r menu_ru_ru.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding koi8-r/' -e 's/" Original translations/" Generated from menu_ru_ru.utf-8.vim, DO NOT EDIT/' > menu_ru_ru.koi8-r.vim

# Convert menu_sl_si.utf-8.vim to create menu_sl_si.cp1250.vim.
menu_sl_si.cp1250.vim: menu_sl_si.utf-8.vim
	rm -f menu_sl_si.cp1250.vim
	iconv -f utf-8 -t cp1250 menu_sl_si.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp1250/'  \
		-e 's/" Original translations/" Generated from menu_sl_si.utf-8.vim, DO NOT EDIT/' > menu_sl_si.cp1250.vim

# Convert menu_uk_ua.utf-8.vim to create menu_sl_si.latin2.vim.
menu_sl_si.latin2.vim: menu_sl_si.utf-8.vim
	rm -f menu_sl_si.latin2.vim
	iconv -f utf-8 -t latin2 menu_sl_si.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding latin2/' -e 's/" Original translations/" Generated from menu_sl_si.utf-8.vim, DO NOT EDIT/' > menu_sl_si.latin2.vim

# Convert menu_uk_ua.utf-8.vim to create menu_slovak_slovak_republic.1250.vim.
menu_slovak_slovak_republic.1250.vim: menu_sl_si.utf-8.vim
	rm -f menu_slovak_slovak_republic.1250.vim
	iconv -f utf-8 -t cp1250 menu_sl_si.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp1250/' -e 's/" Original translations/" Generated from menu_sl_si.utf-8.vim, DO NOT EDIT/' > menu_slovak_slovak_republic.1250.vim

# Convert menu_tr_tr.utf-8.vim to create menu_tr_tr.cp1254.vim.
menu_tr_tr.cp1254.vim: menu_tr_tr.utf-8.vim
	rm -f menu_tr_tr.cp1254.vim
	iconv -f utf-8 -t cp1254 menu_tr_tr.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp1254/' -e 's/" Original translations/" Generated from menu_tr_tr.utf-8.vim, DO NOT EDIT/' > menu_tr_tr.cp1254.vim

# Convert menu_tr_tr.utf-8.vim to create menu_tr_tr.iso_8859-9.vim.
menu_tr_tr.iso_8859-9.vim: menu_tr_tr.utf-8.vim
	rm -f menu_tr_tr.iso_8859-9.vim
	iconv -f utf-8 -t iso8859-9 menu_tr_tr.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding iso8859-9/' -e 's/" Original translations/" Generated from menu_tr_tr.utf-8.vim, DO NOT EDIT/' > menu_tr_tr.iso_8859-9.vim

# Convert menu_sr_rs.utf-8.vim to create menu_sr_rs.iso_8859-5.vim.
menu_sr_rs.iso_8859-5.vim: menu_sr_rs.utf-8.vim
	rm -f menu_sr_rs.iso_8859-5.vim
	iconv -f utf-8 -t iso8859-5 menu_sr_rs.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding iso8859-5/' -e 's/" Original translations/" Generated from menu_sr_rs.utf-8.vim, DO NOT EDIT/' > menu_sr_rs.iso_8859-5.vim

# Convert menu_sr_rs.utf-8.vim to create menu_sr_rs.iso_8859-2.vim.
menu_sr_rs.iso_8859-2.vim: menu_sr_rs.utf-8.vim
	rm -f menu_sr_rs.iso_8859-2.vim
	sed -e 's/??/a/g' -e 's/??/b/g' -e 's/??/v/g' -e 's/??/g/g' -e 's/??/d/g' \
		-e 's/??/??/g' -e 's/??/e/g' -e 's/??/??/g' -e 's/??/z/g' -e 's/??/i/g' \
		-e 's/??/j/g' -e 's/??/k/g' -e 's/??/l/g' -e 's/??/lj/g' -e 's/??/m/g' \
		-e 's/??/n/g' -e 's/??/nj/g' -e 's/??/o/g' -e 's/??/p/g' -e 's/??/r/g' \
		-e 's/??/s/g' -e 's/??/t/g' -e 's/??/??/g' -e 's/??/u/g' -e 's/??/f/g' \
		-e 's/??/h/g' -e 's/??/c/g' -e 's/??/??/g' -e 's/??/d??/g' -e 's/??/??/g' \
		-e 's/??/A/g' -e 's/??/B/g' -e 's/??/V/g' -e 's/??/G/g' -e 's/??/D/g' \
		-e 's/??/??/g' -e 's/??/E/g' -e 's/??/??/g' -e 's/??/Z/g' -e 's/??/I/g' \
		-e 's/??/J/g' -e 's/??/K/g' -e 's/??/L/g' -e 's/??/Lj/g' -e 's/??/M/g' \
		-e 's/??/N/g' -e 's/??/Nj/g' -e 's/??/O/g' -e 's/??/P/g' -e 's/??/R/g' \
		-e 's/??/S/g' -e 's/??/T/g' -e 's/??/??/g' -e 's/??/U/g' -e 's/??/F/g' \
		-e 's/??/H/g' -e 's/??/C/g' -e 's/??/??/g' -e 's/??/D??/g' -e 's/??/??/g' \
		-e 's/scriptencoding utf-8/scriptencoding iso8859-2/' -e 's/" Original translations/" Generated from menu_sr_rs.utf-8.vim, DO NOT EDIT/' \
		menu_sr_rs.utf-8.vim | iconv -f utf-8 -t iso8859-2 \
	> menu_sr_rs.iso_8859-2.vim

# Convert menu_sr_rs.utf-8.vim to create menu_sr_rs.ascii.vim.
menu_sr_rs.ascii.vim: menu_sr_rs.utf-8.vim
	rm -f menu_sr_rs.ascii.vim
	sed -e 's/??/a/g' -e 's/??/b/g' -e 's/??/v/g' -e 's/??/g/g' -e 's/??/d/g' \
		-e 's/??/dj/g' -e 's/??/e/g' -e 's/??/z/g' -e 's/??/z/g' -e 's/??/i/g' \
		-e 's/??/j/g' -e 's/??/k/g' -e 's/??/l/g' -e 's/??/lj/g' -e 's/??/m/g' \
		-e 's/??/n/g' -e 's/??/nj/g' -e 's/??/o/g' -e 's/??/p/g' -e 's/??/r/g' \
		-e 's/??/s/g' -e 's/??/t/g' -e 's/??/c/g' -e 's/??/u/g' -e 's/??/f/g' \
		-e 's/??/h/g' -e 's/??/c/g' -e 's/??/c/g' -e 's/??/dz/g' -e 's/??/s/g' \
		-e 's/??/A/g' -e 's/??/B/g' -e 's/??/V/g' -e 's/??/G/g' -e 's/??/D/g' \
		-e 's/??/??/g' -e 's/??/E/g' -e 's/??/Z/g' -e 's/??/Z/g' -e 's/??/I/g' \
		-e 's/??/J/g' -e 's/??/K/g' -e 's/??/L/g' -e 's/??/Lj/g' -e 's/??/M/g' \
		-e 's/??/N/g' -e 's/??/Nj/g' -e 's/??/O/g' -e 's/??/P/g' -e 's/??/R/g' \
		-e 's/??/S/g' -e 's/??/T/g' -e 's/??/C/g' -e 's/??/U/g' -e 's/??/F/g' \
		-e 's/??/H/g' -e 's/??/C/g' -e 's/??/C/g' -e 's/??/Dz/g' -e 's/??/S/g' \
		-e 's/scriptencoding utf-8/scriptencoding latin1/' -e 's/" Original translations/" Generated from menu_sr_rs.utf-8.vim, DO NOT EDIT/' \
		menu_sr_rs.utf-8.vim > menu_sr_rs.ascii.vim
	
# Convert menu_uk_ua.utf-8.vim to create menu_uk_ua.cp1251.vim.
menu_uk_ua.cp1251.vim: menu_uk_ua.utf-8.vim
	rm -f menu_uk_ua.cp1251.vim
	iconv -f utf-8 -t cp1251 menu_uk_ua.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding cp1251/' -e 's/" Original translations/" Generated from menu_uk_ua.utf-8.vim, DO NOT EDIT/' > menu_uk_ua.cp1251.vim

# Convert menu_uk_ua.utf-8.vim to create menu_uk_ua.koi8-u.vim.
menu_uk_ua.koi8-u.vim: menu_uk_ua.utf-8.vim
	rm -f menu_uk_ua.koi8-u.vim
	iconv -f utf-8 -t koi8-u menu_uk_ua.utf-8.vim | \
		sed -e 's/scriptencoding utf-8/scriptencoding koi8-u/' -e 's/" Original translations/" Generated from menu_uk_ua.utf-8.vim, DO NOT EDIT/' > menu_uk_ua.koi8-u.vim
