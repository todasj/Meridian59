# makefile for libarchive

TOPDIR=..\..
!include $(TOPDIR)\common.mak

# Turn off treating .c files as C++; libarchive code is old-school C
CFLAGS = $(CFLAGS:-TP=-TC) /DHAVE_CONFIG_H

OBJS = \
	$(OUTDIR)\archive_acl.obj \
	$(OUTDIR)\archive_check_magic.obj \
	$(OUTDIR)\archive_cmdline.obj \
	$(OUTDIR)\archive_cryptor.obj \
	$(OUTDIR)\archive_digest.obj \
	$(OUTDIR)\archive_disk_acl_darwin.obj \
	$(OUTDIR)\archive_disk_acl_freebsd.obj \
	$(OUTDIR)\archive_disk_acl_linux.obj \
	$(OUTDIR)\archive_disk_acl_sunos.obj \
	$(OUTDIR)\archive_entry.obj \
	$(OUTDIR)\archive_entry_copy_bhfi.obj \
	$(OUTDIR)\archive_entry_copy_stat.obj \
	$(OUTDIR)\archive_entry_link_resolver.obj \
	$(OUTDIR)\archive_entry_sparse.obj \
	$(OUTDIR)\archive_entry_stat.obj \
	$(OUTDIR)\archive_entry_strmode.obj \
	$(OUTDIR)\archive_entry_xattr.obj \
	$(OUTDIR)\archive_getdate.obj \
	$(OUTDIR)\archive_hmac.obj \
	$(OUTDIR)\archive_match.obj \
	$(OUTDIR)\archive_options.obj \
	$(OUTDIR)\archive_pack_dev.obj \
	$(OUTDIR)\archive_pathmatch.obj \
	$(OUTDIR)\archive_ppmd7.obj \
	$(OUTDIR)\archive_random.obj \
	$(OUTDIR)\archive_rb.obj \
	$(OUTDIR)\archive_read.obj \
	$(OUTDIR)\archive_read_add_passphrase.obj \
	$(OUTDIR)\archive_read_append_filter.obj \
	$(OUTDIR)\archive_read_data_into_fd.obj \
	$(OUTDIR)\archive_read_disk_entry_from_file.obj \
	$(OUTDIR)\archive_read_disk_posix.obj \
	$(OUTDIR)\archive_read_disk_set_standard_lookup.obj \
	$(OUTDIR)\archive_read_disk_windows.obj \
	$(OUTDIR)\archive_read_extract.obj \
	$(OUTDIR)\archive_read_extract2.obj \
	$(OUTDIR)\archive_read_open_fd.obj \
	$(OUTDIR)\archive_read_open_file.obj \
	$(OUTDIR)\archive_read_open_filename.obj \
	$(OUTDIR)\archive_read_open_memory.obj \
	$(OUTDIR)\archive_read_set_format.obj \
	$(OUTDIR)\archive_read_set_options.obj \
	$(OUTDIR)\archive_read_support_filter_all.obj \
	$(OUTDIR)\archive_read_support_filter_bzip2.obj \
	$(OUTDIR)\archive_read_support_filter_compress.obj \
	$(OUTDIR)\archive_read_support_filter_grzip.obj \
	$(OUTDIR)\archive_read_support_filter_gzip.obj \
	$(OUTDIR)\archive_read_support_filter_lrzip.obj \
	$(OUTDIR)\archive_read_support_filter_lz4.obj \
	$(OUTDIR)\archive_read_support_filter_lzop.obj \
	$(OUTDIR)\archive_read_support_filter_none.obj \
	$(OUTDIR)\archive_read_support_filter_program.obj \
	$(OUTDIR)\archive_read_support_filter_rpm.obj \
	$(OUTDIR)\archive_read_support_filter_uu.obj \
	$(OUTDIR)\archive_read_support_filter_xz.obj \
	$(OUTDIR)\archive_read_support_format_7zip.obj \
	$(OUTDIR)\archive_read_support_format_all.obj \
	$(OUTDIR)\archive_read_support_format_ar.obj \
	$(OUTDIR)\archive_read_support_format_by_code.obj \
	$(OUTDIR)\archive_read_support_format_cab.obj \
	$(OUTDIR)\archive_read_support_format_cpio.obj \
	$(OUTDIR)\archive_read_support_format_empty.obj \
	$(OUTDIR)\archive_read_support_format_iso9660.obj \
	$(OUTDIR)\archive_read_support_format_lha.obj \
	$(OUTDIR)\archive_read_support_format_mtree.obj \
	$(OUTDIR)\archive_read_support_format_rar.obj \
	$(OUTDIR)\archive_read_support_format_raw.obj \
	$(OUTDIR)\archive_read_support_format_tar.obj \
	$(OUTDIR)\archive_read_support_format_warc.obj \
	$(OUTDIR)\archive_read_support_format_xar.obj \
	$(OUTDIR)\archive_read_support_format_zip.obj \
	$(OUTDIR)\archive_string.obj \
	$(OUTDIR)\archive_string_sprintf.obj \
	$(OUTDIR)\archive_util.obj \
	$(OUTDIR)\archive_version_details.obj \
	$(OUTDIR)\archive_virtual.obj \
	$(OUTDIR)\archive_windows.obj \
	$(OUTDIR)\archive_write.obj \
	$(OUTDIR)\archive_write_add_filter.obj \
	$(OUTDIR)\archive_write_add_filter_b64encode.obj \
	$(OUTDIR)\archive_write_add_filter_by_name.obj \
	$(OUTDIR)\archive_write_add_filter_bzip2.obj \
	$(OUTDIR)\archive_write_add_filter_compress.obj \
	$(OUTDIR)\archive_write_add_filter_grzip.obj \
	$(OUTDIR)\archive_write_add_filter_gzip.obj \
	$(OUTDIR)\archive_write_add_filter_lrzip.obj \
	$(OUTDIR)\archive_write_add_filter_lz4.obj \
	$(OUTDIR)\archive_write_add_filter_lzop.obj \
	$(OUTDIR)\archive_write_add_filter_none.obj \
	$(OUTDIR)\archive_write_add_filter_program.obj \
	$(OUTDIR)\archive_write_add_filter_uuencode.obj \
	$(OUTDIR)\archive_write_add_filter_xz.obj \
	$(OUTDIR)\archive_write_disk_posix.obj \
	$(OUTDIR)\archive_write_disk_set_standard_lookup.obj \
	$(OUTDIR)\archive_write_disk_windows.obj \
	$(OUTDIR)\archive_write_open_fd.obj \
	$(OUTDIR)\archive_write_open_file.obj \
	$(OUTDIR)\archive_write_open_filename.obj \
	$(OUTDIR)\archive_write_open_memory.obj \
	$(OUTDIR)\archive_write_set_format.obj \
	$(OUTDIR)\archive_write_set_format_7zip.obj \
	$(OUTDIR)\archive_write_set_format_ar.obj \
	$(OUTDIR)\archive_write_set_format_by_name.obj \
	$(OUTDIR)\archive_write_set_format_cpio.obj \
	$(OUTDIR)\archive_write_set_format_cpio_newc.obj \
	$(OUTDIR)\archive_write_set_format_filter_by_ext.obj \
	$(OUTDIR)\archive_write_set_format_gnutar.obj \
	$(OUTDIR)\archive_write_set_format_iso9660.obj \
	$(OUTDIR)\archive_write_set_format_mtree.obj \
	$(OUTDIR)\archive_write_set_format_pax.obj \
	$(OUTDIR)\archive_write_set_format_raw.obj \
	$(OUTDIR)\archive_write_set_format_shar.obj \
	$(OUTDIR)\archive_write_set_format_ustar.obj \
	$(OUTDIR)\archive_write_set_format_v7tar.obj \
	$(OUTDIR)\archive_write_set_format_warc.obj \
	$(OUTDIR)\archive_write_set_format_xar.obj \
	$(OUTDIR)\archive_write_set_format_zip.obj \
	$(OUTDIR)\archive_write_set_options.obj \
	$(OUTDIR)\archive_write_set_passphrase.obj \
	$(OUTDIR)\filter_fork_posix.obj \
	$(OUTDIR)\filter_fork_windows.obj \
	$(OUTDIR)\xxhash.obj

all: makedirs $(BLAKLIBDIR)\libarchive.lib

$(BLAKLIBDIR)\libarchive.lib: $(OBJS)
	$(LIBPRG) $** $(LIBS) -out:$@

!include $(TOPDIR)\rules.mak
