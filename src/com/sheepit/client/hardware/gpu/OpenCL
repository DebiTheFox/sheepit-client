/*
 * Copyright (C) 2013-2014 Laurent CLOUET
 * Author Laurent CLOUET <laurent.clouet@nopnop.net>
 *
 * This program is free software; you can redistribute it and/or 
 * modify it under the terms of the GNU General Public License
 * as published by the Free Software Foundation; version 2
 * of the License.
 *
 * This program is distributed in the hope that it will be useful,
 * but WITHOUT ANY WARRANTY; without even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License
 * along with this program; if not, write to the Free Software
 * Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 */

package com.sheepit.client.hardware.gpu;

import com.sun.jna.Library;
import com.sun.jna.ptr.IntByReference;
import com.sun.jna.ptr.LongByReference;

public interface OpenCL extends Library {
	public int opInit(int flags);
	
	/*
	 * @return: OpenCL_SUCCESS, OpenCL_ERROR_DEINITIALIZED, OpenCL_ERROR_NOT_INITIALIZED, OpenCL_ERROR_INVALID_CONTEXT, OpenCL_ERROR_INVALID_VALUE 
	*/
	public int opDeviceGetCount(IntByReference count);
	
	public int opDeviceGetName(byte[] name, int len, int dev);
	
	public int opDeviceTotalMem_v2(LongByReference bytes, int dev);
	public int opDeviceTotalMem(LongByReference bytes, int dev);
}
