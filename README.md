import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { motion } from "framer-motion";
import { Mail, Phone, Github, MapPin } from "lucide-react";

export default function PersonalCV() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-sky-100 via-indigo-100 to-purple-100 text-slate-800 p-6">
      <div className="max-w-6xl mx-auto space-y-8">

        {/* Header */}
        <motion.div
          initial={{ opacity: 0, y: 40 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.6 }}
        >
          <Card className="bg-white/80 backdrop-blur border border-white/50 rounded-2xl shadow-xl">
            <CardContent className="p-8 flex flex-col md:flex-row items-center gap-8">
              <div className="w-40 h-40 rounded-full bg-gradient-to-tr from-sky-400 via-indigo-400 to-purple-400 flex items-center justify-center text-4xl font-bold text-white shadow-lg">
                Q
              </div>

              <div className="space-y-3 text-center md:text-left">
                <h1 className="text-4xl font-bold text-slate-900">Quan Nguyen</h1>
                <p className="text-xl text-indigo-600 font-semibold">
                  Game Developer / Unity Developer
                </p>
                <p className="text-slate-600 max-w-xl">
                  Passionate developer focusing on gameplay systems, performance optimization,
                  and interactive experiences. Experienced in Unity, C#, and game architecture design.
                </p>
              </div>
            </CardContent>
          </Card>
        </motion.div>

        {/* Contact */}
        <motion.div
          initial={{ opacity: 0, y: 40 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ delay: 0.1 }}
        >
          <Card className="bg-white/80 backdrop-blur border border-white/50 rounded-2xl shadow-xl">
            <CardContent className="p-6 grid md:grid-cols-2 lg:grid-cols-4 gap-6">
              <div className="flex items-center gap-3 bg-sky-50 p-3 rounded-xl">
                <Mail className="w-5 h-5 text-sky-500" />
                <span>your@email.com</span>
              </div>

              <div className="flex items-center gap-3 bg-indigo-50 p-3 rounded-xl">
                <Phone className="w-5 h-5 text-indigo-500" />
                <span>+84 xxx xxx xxx</span>
              </div>

              <div className="flex items-center gap-3 bg-purple-50 p-3 rounded-xl">
                <Github className="w-5 h-5 text-purple-500" />
                <span>github.com/yourname</span>
              </div>

              <div className="flex items-center gap-3 bg-pink-50 p-3 rounded-xl">
                <MapPin className="w-5 h-5 text-pink-500" />
                <span>Ha Noi, Viet Nam</span>
              </div>
            </CardContent>
          </Card>
        </motion.div>

        {/* Skills + Experience */}
        <div className="grid md:grid-cols-2 gap-8">

          {/* Skills */}
          <motion.div
            initial={{ opacity: 0, y: 40 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ delay: 0.2 }}
          >
            <Card className="bg-white/80 backdrop-blur border border-white/50 rounded-2xl shadow-xl">
              <CardContent className="p-6 space-y-4">
                <h2 className="text-2xl font-bold text-indigo-700">Skills</h2>
                <ul className="space-y-2 text-slate-600">
                  <li>• Unity Engine</li>
                  <li>• C# Programming</li>
                  <li>• Gameplay System Design</li>
                  <li>• Performance Optimization</li>
                  <li>• Git / Version Control</li>
                </ul>
              </CardContent>
            </Card>
          </motion.div>

          {/* Experience */}
          <motion.div
            initial={{ opacity: 0, y: 40 }}
            animate={{ opacity: 1, y: 0 }}
            transition={{ delay: 0.3 }}
          >
            <Card className="bg-white/80 backdrop-blur border border-white/50 rounded-2xl shadow-xl">
              <CardContent className="p-6 space-y-4">
                <h2 className="text-2xl font-bold text-purple-700">Experience</h2>
                <div className="space-y-3">
                  <div className="bg-purple-50 p-4 rounded-xl">
                    <p className="font-semibold text-slate-800">Game Developer</p>
                    <p className="text-slate-500 text-sm">Company Name • 2023 - Present</p>
                    <p className="text-slate-600 text-sm">
                      Developed gameplay systems, optimized performance, and implemented game mechanics.
                    </p>
                  </div>
                </div>
              </CardContent>
            </Card>
          </motion.div>

        </div>

        {/* Education */}
        <motion.div
          initial={{ opacity: 0, y: 40 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ delay: 0.4 }}
        >
          <Card className="bg-white/80 backdrop-blur border border-white/50 rounded-2xl shadow-xl">
            <CardContent className="p-6 space-y-4">
              <h2 className="text-2xl font-bold text-sky-700">Education</h2>
              <div className="bg-sky-50 p-4 rounded-xl">
                <p className="font-semibold text-slate-800">Your University</p>
                <p className="text-slate-500 text-sm">Major • Year - Year</p>
              </div>
            </CardContent>
          </Card>
        </motion.div>

        {/* Footer */}
        <div className="text-center text-slate-500 text-sm pt-4">
          © {new Date().getFullYear()} Quan Nguyen
        </div>

      </div>
    </div>
  );
}
